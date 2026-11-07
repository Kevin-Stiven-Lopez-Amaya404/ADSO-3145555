# Respuesta a las 14 correcciones del instructor — SmartHome

**SENA · Ficha ADSO 3145555 · Revisión: 7 de noviembre de 2026**

El alcance del informe es **documental y administrativo**. No declara pruebas técnicas, autorizaciones ni tags como completados sin evidencia.

| # | Requisito del instructor | Estado verificable | Acción final |
|---|---|---|---|
| 1 | Release `final-delivery` con dos ZIP por repo | **Parcial.** Release publicado [aquí](https://github.com/Kevin-Stiven-Lopez-Amaya404/ADSO-3145555/releases/tag/final-delivery), solo un Asset `SmartHome.zip` | Cargar 10 ZIP reales y SHA-256 por cada repo; revisar que coincidan con tag `final-delivery-2026` |
| 2 | Un PR, no #13 y #17 | **Consolidado en contenido.** PR #17 incorpora los cuatro archivos binarios de #13 con trazabilidad; ambos siguen abiertos | Autora de #13 debe verificar y cerrar #13 sin fusionarlo; aprobar #17 |
| 3 | Archivo Drive restringido | **Pendiente**. No se identificó de manera fiable cuál falla para usuarios sin sesión. | Propietario: `Compartir → Acceso general → Cualquier persona con enlace → Lector`; probar con incógnito. No dar Editor público |
| 4 | SRS final en sección 01 | **Subido:** [PDF](01-requirements-specification/requirements-specification.pdf) y [fuente](01-requirements-specification/source-reference.md) | Instructor verifica versión y legibilidad |
| 5 | PDF secciones 02/04/05/06/09 | **Subidos** y enlaces en [inventario](DOCUMENTACION-DEL-RELEASE.md) | Instructor verifica contenido, firma/portada, y aprueba |
| 6 | Dos repos de documentación | **Aclarado** en [code-tag](code-tag/README.md): `smart-home-doc` canónico; `smart-home-docs` antiguo de un solo archivo | Cumplir además el requisito explícito del instructor de etiquetar/exportar el antiguo, o pedir autorización para cambiarlo |
| 7 | Pitch/tutorial y duración | **No conformes**: videos originales web 06:29 y Android 10:05; ambos exceden tutorial 3–5 min, ninguno validado pitch | Publicar pitch 1–2 min y tutorial 3–5 min, revisar privacidad y confirmar duración en [10-videos](10-videos/README.md) |
| 8 | Tag `final-delivery-2026` + dos ZIP × 5 repos | **Pendiente**: tag no encontrado en ninguno de los cinco repos revisados | Aprobar estado de `main`, etiquetar con tag anotado y exportar snapshot + espejo Git; generar hashes reales |
| 9 | Autorizar datos 3/3 en README | **Pendiente**: las 3 casillas sin marcar | Cada integrante debe verificar su información y consentir expresamente; nunca marcar por terceros |
| 10 | Rol completo 3/3 en `team-roster.md` | **Diligenciado como propuesta** con roles documentados, **pendiente ratificación** | Cada integrante confirma o corrige su rol |
| 11 | Aporte completo 3/3 en `software-registration.md` | **Diligenciado como propuesta**, pendiente confirmación de contribución individual | Cada integrante valida su aporte para registro de software |
| 12 | Ocho campos secciones 5 y 6 | **Parcial**: funciones, lenguajes, plataforma y descripción están diligenciados; origen, clase de obra, publicación y fecha deben declararse por titulares | Completar con autores/instructor. No inventar decisiones de derechos de autor |
| 13 | Fecha y entregante en README | **Diligenciado** (07-11-2026 como fecha de preparación; Kevin Stiven López Amaya como entregante) | Actualizar fecha real de entrega al publicar |
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
