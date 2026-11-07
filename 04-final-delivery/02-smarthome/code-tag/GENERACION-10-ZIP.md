# Procedimiento reproducible — cinco tags y diez ZIP de SmartHome

**ADSO 3145555 — revisión técnica 7 de noviembre de 2026**

## Estado real

- El [Release `final-delivery`](https://github.com/Kevin-Stiven-Lopez-Amaya404/ADSO-3145555/releases/tag/final-delivery) del fork está **publicado**, pero únicamente contiene el Asset documental `SmartHome.zip`.
- No se encontró `final-delivery-2026` en ninguno de los cinco repositorios del instructor al revisar.
- El `main` móvil (`f1deb5331a07ef51dae213a20aa48c2a52fe1027`) es histórico y requiere la aprobación de QA/Android físico.
- El `main` web (`daae7a411c0da213ff078e9ae6fde67d9f29702b`) tuvo una [CI fallida](https://github.com/nataliachala1/smarthome-frontend-web/actions/runs/42114983557).
- Por tanto, los cinco tags y diez ZIP **no están aprobados ni publicados**; no crear etiquetas sin congelar versiones válidas.

## Repositorios exactos indicados por el instructor

1. `Kevin-Stiven-Lopez-Amaya404/from_movil`
2. `Kevin-Stiven-Lopez-Amaya404/smart-home-docs`
3. `nataliachala1/smart-home-database`
4. `nataliachala1/smarthome-backend`
5. `nataliachala1/smarthome-frontend-web`

`smart-home-docs` y `smart-home-database` son repositorios antiguos que forman parte de los cinco explícitos del instructor; **no omitirlos**. La documentación canónica es `smart-home-doc` y la BD canónica es `smarthome-database`. Solicitar autorización si se van a añadir ambos como sexto/séptimo paquete.

## Método de empaquetado y trazabilidad

Para **cada** repositorio, solo una vez que su `main` esté aprobado:

1. Crear y publicar un **tag anotado** `final-delivery-2026` sobre el SHA exacto de `main`.
2. Verificar `git ls-remote origin 'refs/tags/final-delivery-2026^{}'` contra el SHA aprobado.
3. Exportar snapshot: `git archive --format=zip --output=<repo>-final-delivery-2026-main.zip final-delivery-2026`.
4. Crear espejo completo con `git clone --mirror`; ejecutar `git fsck --full`.
5. Crear `git bundle create <repo>.bundle --all` y verificarlo con `git bundle verify`. Después restaurar el bundle en un directorio Git espejo independiente, ejecutar `git fsck --full` y comparar los SHA de todas las ramas/tags contra el espejo original.
6. Empaquetar ese bundle, manifest de referencias y `RESTAURAR.txt` dentro de `<repo>-full-export.zip`.
7. Calcular el SHA-256 de **ambos ZIP** y registrarlo en `SHA256SUMS.txt`; verificar los ZIP.
8. Subir los diez ZIP como Assets del Release **ya existente** y actualizar [code-tag/README.md](README.md) con enlaces y hashes reales.

Se preparó un script de PowerShell para automatizar el proceso en Windows con controles de SHA y aprobación expresa. **No se ha ejecutado contra los repositorios**: el entorno de trabajo actual no dispone de acceso Git de red para clonar paquetes completos. Debe ejecutarlo un integrante autorizado en un equipo con conexión a GitHub.

## Derechos de acceso

El instructor `ariel5253` necesita **Write** en los cinco repositorios. `from_movil` y `smart-home-docs` devolvieron permiso `Read` durante la revisión; para los otros tres hay que comprobar permisos desde la cuenta propietaria.

## Aceptación final

Marcar esta sección como completa **únicamente** si hay cinco tags anotados que apuntan al `main` aprobado, diez ZIP descargables (cada uno con integridad verificada), diez SHA-256 registrados, revisión de CI/QA y acceso de escritura del instructor.

**Comprobación local de la metodología (7 de noviembre de 2026):** la secuencia `git archive` + `git bundle --all` + restauración espejo fue probada con un repositorio de Git temporal con `main`, `dev` y un tag anotado, y sus tres referencias conservaron sus SHA. **Esta prueba no valida aún los cinco repositorios reales ni implica que sus tags hayan sido creados.**
