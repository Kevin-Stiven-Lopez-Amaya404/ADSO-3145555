# Respuesta a las 14 correcciones del instructor — SmartHome

**SENA · Ficha ADSO 3145555 · Revisión: 7 de noviembre de 2026**

El alcance del informe es **documental y administrativo**. No declara pruebas técnicas, autorizaciones ni tags como completados sin evidencia.

| # | Requisito del instructor | Estado verificable | Acción final |
|---|---|---|---|
| 1 | Release `final-delivery` con dos ZIP por repo | **Parcial.** Release publicado [aquí](https://github.com/Kevin-Stiven-Lopez-Amaya404/ADSO-3145555/releases/tag/final-delivery), solo un Asset `SmartHome.zip` | Cargar 10 ZIP reales y SHA-256 por cada repo; revisar que coincidan con tag `final-delivery-2026` |
| 2 | Un PR, no #13 y #17 | **Consolidado en contenido.** PR #17 incorpora los cuatro archivos binarios de #13 con trazabilidad; ambos siguen abiertos | Autora de #13 debe verificar y cerrar #13 sin fusionarlo; PR #5 ya fue cerrado sin fusionar; aprobar #17 |
| 3 | Archivo Drive restringido | **Pendiente**. No se identificó de manera fiable cuál falla para usuarios sin sesión. | Revisión privada de permisos: configurar `Compartir → Acceso general → Cualquier persona con enlace → Lector` en la carpeta y los archivos; probar con incógnito. [Guía](AUDITORIA-ACCESO-DRIVE.md) |
| 4 | SRS final en sección 01 | **Subido:** [PDF](01-requirements-specification/requirements-specification.pdf) y [fuente](01-requirements-specification/source-reference.md) | Instructor verifica versión y legibilidad |
| 5 | PDF secciones 02/04/05/06/09 | **Subidos** y enlaces en [inventario](DOCUMENTACION-DEL-RELEASE.md) | Instructor verifica contenido, firma/portada, y aprueba |
| 6 | Dos repos de documentación | **Aclarado** en [code-tag](code-tag/README.md): `smart-home-doc` canónico; `smart-home-docs` antiguo de un solo archivo | Cumplir además el requisito explícito del instructor de etiquetar/exportar el antiguo, o pedir autorización para cambiarlo |
| 7 | Pitch/tutorial y duración | **No conformes**: videos originales web 06:29 y Android 10:05; ambos exceden tutorial 3–5 min, ninguno validado pitch | Publicar pitch 1–2 min y tutorial 3–5 min, revisar privacidad y confirmar duración en [10-videos](10-videos/README.md) |
| 8 | Tag `final-delivery-2026` + dos ZIP × 5 repos | **Pendiente**: tag no encontrado en ninguno de los cinco repos revisados | Aprobar estado de `main`, etiquetar con tag anotado y exportar snapshot + espejo Git; generar hashes reales |
| 9 | Autorizar datos 3/3 en README | **Pendiente**: las 3 casillas sin marcar | Cada integrante debe verificar su información y consentir expresamente; nunca marcar por terceros |
| 10 | Rol completo 3/3 en `team-roster.md` | **Diligenciado como propuesta** con roles documentados, **pendiente ratificación** | Cada integrante confirma o corrige su rol |
| 11 | Aporte completo 3/3 en `software-registration.md` | **Diligenciado como propuesta**, pendiente confirmación de contribución individual | Cada integrante valida su aporte para registro de software |
| 12 | Ocho campos secciones 5 y 6 | **Parcial**: funciones, lenguajes, plataforma y descripción están diligenciados; origen, clase de obra, publicación y fecha deben declararse por titulares | Completar con autores/instructor. No inventar decisiones de derechos de autor |
| 13 | Fecha y entregante en README | **Diligenciado** (07-11-2026 como fecha de preparación; Kevin Stiven López Amaya como entregante) | El Release documental ya fue publicado 07-11-2026, pero la entrega técnica sigue pendiente de aceptación del instructor |
| 14 | Acceso Write de `ariel5253` en 5 repos | **Pendiente**: `from_movil` y `smart-home-docs` muestran Read, otras 3 consultas no verificables por esta integración | Propietarios: Settings → Collaborators → cambiar/otorgar **Write**; revisar invitación aceptada |

## Repositorios de los cinco paquetes solicitados

1. `Kevin-Stiven-Lopez-Amaya404/from_movil`
2. `Kevin-Stiven-Lopez-Amaya404/smart-home-docs` (histórico, exigido por instructor)
3. `nataliachala1/smart-home-database` (histórico, exigido por instructor)
4. `nataliachala1/smarthome-backend`
5. `nataliachala1/smarthome-frontend-web`

**Observación importante:** el repositorio canónico de datos del proyecto es `nataliachala1/smarthome-database`, diferente de `smart-home-database`. El canónico documental es `Kevin-Stiven-Lopez-Amaya404/smart-home-doc`. El instructor debe decidir si se agregan como sexto/séptimo repositorio además de los cinco explícitos. No sustituirlos silenciosamente.

## Publicación e integridad

El GitHub Release del fork ya está publicado con un ZIP de documentación. Los diez ZIP de código **no** constan como Assets todavía; el tag del Release del fork (`final-delivery`) es **distinto** al tag de los cinco repos (`final-delivery-2026`). En `code-tag/SHA256SUMS.txt` se deben escribir únicamente hashes calculados de los ZIP finales descargables.

**Pendientes ajenos a la documentación:** cierre de CI frontend web, revisión de seguridad móvil y prueba física Android. No se considera aprobado un commit `main` hasta cumplir los controles que correspondan.

## Avances posteriores a la lista inicial

- El [PR #5](https://github.com/code-sena/ADSO-3145555/pull/5) fue **cerrado sin fusionar** por el autor, para retirar de evaluación los 546 archivos ajenos a la entrega de SmartHome.
- El [README](README.md) identifica cuáles PDF ya están incorporados para revisión y separa la versión documental de los tags técnicos aún pendientes.
- Se publicó una [guía de control de acceso a Drive](AUDITORIA-ACCESO-DRIVE.md) que exige permisos públicos de lectura, sin publicar detalles sensibles de seguridad.
- El [procedimiento de generación de diez ZIP](code-tag/GENERACION-10-ZIP.md) está preparado y existe un paquete PowerShell para Windows. **No se han producido los diez ZIP de código ni sus tags anotados** mientras haya commits sin aprobación.
- El [Release `final-delivery`](https://github.com/Kevin-Stiven-Lopez-Amaya404/ADSO-3145555/releases/tag/final-delivery) **ya está publicado**, con un Asset documental. Su descripción y Assets deben actualizarse con los paquetes de código verificables antes de considerarlo final.

**No confundir documento enviado, archivo disponible, PR aprobado y Release técnico validado: son estados distintos.**


## Verificación de integración y aceptación — cierre de revisión

**Comprobación de GitHub del 7 de noviembre de 2026:**

- [PR institucional #17](https://github.com/code-sena/ADSO-3145555/pull/17): **OPEN**, **mergeable: clean**. Puede ser revisado por el mantenedor, pero todavía **no está fusionado**.
- [PR institucional #13](https://github.com/code-sena/ADSO-3145555/pull/13): **OPEN**; sus archivos están incorporados al #17, pero debe cerrarlo su autora. Un intento de cierre con la cuenta conectada fue rechazado con **403**.
- [PR móvil #61](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/pull/61): **DRAFT**, clean, pruebas automáticas de CI aprobadas en el candidato SDK 58. **No equivale a aceptación física Android**.
- [PR móvil #49](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/pull/49): **DRAFT**, estado de integración unstable, aún no aprobado para `main`.
- [PR #7 web en el fork](https://github.com/Kevin-Stiven-Lopez-Amaya404/smarthome-frontend-web/pull/7): **MERGED** en `dev` de la copia, commit `9928217825c79cf8150b0dd97ce2937c1d95603d`; [CI antes](https://github.com/Kevin-Stiven-Lopez-Amaya404/smarthome-frontend-web/actions/runs/42395316954) y [después](https://github.com/Kevin-Stiven-Lopez-Amaya404/smarthome-frontend-web/actions/runs/42395677610) de fusionar: **SUCCESS**. La corrección **no está integrada en el upstream web**.
- [Release documental del fork](https://github.com/Kevin-Stiven-Lopez-Amaya404/ADSO-3145555/releases/tag/final-delivery): publicado, con **un solo Asset `SmartHome.zip`**. El instructor solicita dos ZIP por cada uno de cinco repositorios, que siguen pendientes.

### Advertencia administrativa

La preparación de un ZIP, un script o una prueba CI en un fork **no son prueba de la entrega final de `main` de cada repositorio**. Para cumplir el requisito de registro del software deben identificarse SHA aprobados, tags anotados, diez ZIP de snapshot y exportación completa, hashes SHA-256 auténticos y enlaces de Asset descargables. Las autorizaciones de datos y declaraciones legales deben ser voluntarias y verificadas por los integrantes.
