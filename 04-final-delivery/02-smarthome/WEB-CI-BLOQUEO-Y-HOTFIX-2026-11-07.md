# SmartHome — Bloqueo de CI web y hotfix pendiente de integrar

**Fecha:** 7 de noviembre de 2026. **Estado:** diagnóstico confirmado; corrección verificada en fork; no fusionada al repositorio original.

## Falla verificada

- Repositorio original: [nataliachala1/smarthome-frontend-web](https://github.com/nataliachala1/smarthome-frontend-web), `main` SHA `daae7a411c0da213ff078e9ae6fde67d9f29702b`.
- [Workflow fallido](https://github.com/nataliachala1/smarthome-frontend-web/actions/runs/42114983557): `validate`, paso `Smoke test frontend container`, fallido; lint, TypeScript, pruebas de contrato, build Vite y construcción Docker aprobados.
- Error de Nginx en el log: `host not found in upstream "smart-home-smarthomebackendprod-jre7g6"`.
- El workflow de `dev` del upstream solo incluye el alias `backend=127.0.0.1` durante el smoke.

## Solución exacta

En `.github/workflows/ci-deploy.yml`, sustituir el comando `docker run` de la prueba de humo por:

```bash
docker run --detach --add-host backend=127.0.0.1 --add-host smart-home-smarthomebackendprod-jre7g6=127.0.0.1 --name smarthome-frontend-web-ci --publish 127.0.0.1:18080:8080 smarthome-frontend-web:ci
```

El alias se aplica **solo al contenedor de la prueba CI**; no habilita deploy, no modifica Nginx de producción ni prueba que el backend real responda.

## Evidencia y autorización

- [PR #7 del fork](https://github.com/Kevin-Stiven-Lopez-Amaya404/smarthome-frontend-web/pull/7) contiene exactamente este cambio y está fusionado a `dev` del fork.
- [CI del fork](https://github.com/Kevin-Stiven-Lopez-Amaya404/smarthome-frontend-web/actions/runs/42395677610) finalizó con `validate` **success** y smoke healthy.
- Intentos de crear una rama y abrir PR directamente en el upstream de Natalia con la integración conectada: **403 Resource not accessible by integration**. No se modificó el upstream.
- Acción de Natalia o un colaborador con Write: crear rama hija de `dev`, aplicar el parche, abrir PR a `dev`, validar y promover mediante `qa` y `main` con la aprobación correspondiente.

**No crear el tag `final-delivery-2026` sobre el `main` web fallido.** El paquete local `SmartHome_Web_CI_Hotfix_2026-11-07.zip` contiene el parche y las instrucciones para PowerShell; no está publicado como Asset del Release.
