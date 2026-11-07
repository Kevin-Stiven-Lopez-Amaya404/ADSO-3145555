# SmartHome — Inventario de entrega académica
**SENA · ADSO 3145555 · Revisión 7 de noviembre de 2026**

Este inventario consolida en el **PR #17** los archivos originalmente aportados en el PR #13 por Karen Daniela Holguín Cruz y los informes técnicos subidos por Kevin Stiven López Amaya. La incorporación a `code-sena/main` continúa sujeta a aprobación institucional.

## Archivos requeridos y sus PDF

| Sección institucional | PDF final en este PR | Fuente editable o material de apoyo |
|---|---|---|
| 01 Requisitos | [requirements-specification.pdf](01-requirements-specification/requirements-specification.pdf) | [Referencia SRS](01-requirements-specification/source-reference.md), archivo Markdown original en la carpeta Drive |
| 02 Análisis de software | [02-software-analysis.pdf](02-software-analysis/02-software-analysis.pdf) | [Markdown](02-software-analysis/02-software-analysis.md) |
| 03 Propuesta técnica | [03-technical-proposal.pdf](03-technical-proposal/03-technical-proposal.pdf) | [Word actualizado](03-technical-proposal/03-technical-proposal.docx) y Word histórico del PR #13 (conservado) |
| 04 Diseño de software | [04-software-design.pdf](04-software-design/04-software-design.pdf) | [Markdown](04-software-design/04-software-design.md), Word original en carpeta Drive |
| 05 Pruebas | [05-test-documentation.pdf](05-test-documentation/05-test-documentation.pdf) · [Protocolo QA Android/Shelly](05-test-documentation/qa-android-shelly-2026-11-07.pdf) | [Markdown general](05-test-documentation/05-test-documentation.md), [protocolo con 18 casos](05-test-documentation/qa-android-shelly-2026-11-07.md) y [registro CSV pendiente](05-test-documentation/qa-android-shelly-registro-2026-11-07.csv) |
| 06 Procedimiento de implementación | [06-implementation-procedure.pdf](06-implementation-procedure/06-implementation-procedure.pdf) | [Markdown](06-implementation-procedure/06-implementation-procedure.md) |
| 07 Acciones correctivas y mejora | [07-improvement-actions.pdf](07-improvement-actions/07-improvement-actions.pdf) | [Markdown actualizado](07-improvement-actions/07-improvement-actions.md), [Word editable](07-improvement-actions/07-improvement-actions.docx) y Word histórico del PR #13 |
| 08 Manuales | [Manual técnico](08-manuals/technical-manual.pdf) · [Instalación](08-manuals/installation-manual.pdf) · [Usuario final](08-manuals/end-user-manual.pdf) | DOCX y Markdown editables de cada manual en [08-manuals](08-manuals/); anexo ISO histórico del PR #13 conservado |
| 09 Artículo | [09-project-article.pdf](09-project-article/09-project-article.pdf) | [Markdown](09-project-article/09-project-article.md), PDF original del PR #13 |
| 10 Videos | [Videos verificados](10-videos/video-links.md) | Dos propuestas de 01:30 y 04:45 preparadas en Drive privado; faltan aprobación y acceso lector público |
| code-tag | [Estado de repositorios y tags](code-tag/README.md) | Falta aprobar tags, generar diez ZIP y calcular SHA-256 reales |
| Registro | [Equipo](team-roster.md) · [Registro software](software-registration.md) | Roles y aportes documentados para ratificación; autorizaciones de datos aún sin marcar |

## Archivos originales y paquete opcional para Release

[Carpeta original de Google Drive](https://drive.google.com/drive/folders/1FI2E_qAiMVAG1lDXIPhSyPoFF3Pc8ndQ): contiene 15 archivos en 12 secciones, además de sus duplicados históricos. El paquete local `SmartHome_Release_Todo.zip` combina los 15 originales de Drive con los 37 archivos documentales preparados previamente. **Un ZIP de documentos no sustituye los diez ZIP de código obligatorios.**

## Presentación de un solo PR

- [PR #17](https://github.com/code-sena/ADSO-3145555/pull/17) contiene los cinco archivos del [PR #13](https://github.com/code-sena/ADSO-3145555/pull/13) sin alterar su autoría original. Se solicita a la autora del PR #13 cerrarlo tras validar la consolidación para mantener un único PR activo de SmartHome.
- El [PR #5](https://github.com/code-sena/ADSO-3145555/pull/5) tiene cambios ajenos a este proyecto y no debe integrarse como entrega final.
- La entrega necesita aprobación institucional; los permisos de la cuenta conectada impiden fusionar en `code-sena/main`.

**Estado documental al 07-11-2026:** PDF académicos 01/02/03/04/05/06/07/08 (tres manuales)/09 disponibles en la rama del PR #17; pendientes de revisión y fusión institucional. Los videos, los tags y los diez ZIP técnicos todavía no están acreditados. Los archivos históricos se conservan por trazabilidad.

## Evidencia de corrección web (7 de noviembre de 2026)

- [PR #7 en fork web](https://github.com/Kevin-Stiven-Lopez-Amaya404/smarthome-frontend-web/pull/7): **fusionado en `dev` del fork**; commit `9928217825c79cf8150b0dd97ce2937c1d95603d`.
- [CI de la rama de corrección: SUCCESS](https://github.com/Kevin-Stiven-Lopez-Amaya404/smarthome-frontend-web/actions/runs/42395316954).
- [CI de `dev` tras la fusión: SUCCESS](https://github.com/Kevin-Stiven-Lopez-Amaya404/smarthome-frontend-web/actions/runs/42395677610).
- **Pendiente en `nataliachala1/smarthome-frontend-web`:** introducir y verificar el mismo cambio en `dev`, promoverlo con aprobación por `qa` a `main` y confirmar smoke del `main` antes de crear el tag final. La conexión de Stiven no tiene permiso para crear ese PR en upstream (403).

## Acciones mínimas que siguen impidiendo la evaluación definitiva

| Responsable | Acción verificable | Estado |
|---|---|---|
| Natalia (propietaria de repositorios) | Revisar corrección web en upstream; aprobar CI web y las versiones de `main` | Pendiente |
| Equipo móvil | Probar APK/flujo físico Android, revisar PR #61 y PR #49 antes de promover `main` | Pendiente |
| Daniela | Confirmar que sus 5 archivos de #13 aparecen en #17 y cerrar #13 **sin fusionar** | Pendiente; la cuenta conectada recibió 403 al intentar cerrar |
| Instructor/mantenedor institucional | Revisar y fusionar PR #17 | Pendiente; 403 para la cuenta de Stiven |
| Propietarios de Drive | Configurar enlaces `Cualquier persona con enlace → Lector` y probar acceso anónimo | Pendiente de comprobación |
| Integrantes (cada uno) | Ratificar rol y aportes, y consentir voluntariamente la publicación de datos | Pendiente 3/3 |
| Propietarios de 5 repositorios | Otorgar `Write` a `ariel5253`; congelar commits `main`, publicar 5 tags y 10 ZIP con hashes | Pendiente |
| Equipo audiovisual | Confirmar pitch 01–02 min y tutorial 03–05 min accesibles mediante enlaces lectores | Pendiente |

**Release real:** [`final-delivery` publicado](https://github.com/Kevin-Stiven-Lopez-Amaya404/ADSO-3145555/releases/tag/final-delivery), todavía con un único Asset documental `SmartHome.zip`. No equivale a la entrega verificada de cinco repositorios.


## Bloqueo CI web del upstream (7-11-2026)

El [diagnóstico y hotfix reproducible](WEB-CI-BLOQUEO-Y-HOTFIX-2026-11-07.md) confirma que la CI de `main` del repositorio original falla al iniciar Nginx porque no resuelve el alias interno del backend. La misma corrección está validada en el fork, pero **no pudo abrirse PR en upstream por respuesta 403** de la integración. Natalia (o un colaborador con Write) debe aplicar el parche a una rama de `dev`, validar PR/QA y promover a `main` antes de etiquetar. No se ha fusionado ni modificado el repositorio original.


## Complemento QA Android / Shelly (7-11-2026)

Se añadieron al producto **05 Pruebas** un [protocolo PDF](05-test-documentation/qa-android-shelly-2026-11-07.pdf), [fuente Markdown](05-test-documentation/qa-android-shelly-2026-11-07.md) y [matriz CSV de 18 casos](05-test-documentation/qa-android-shelly-registro-2026-11-07.csv). La APK **debug** de [QA `6c3946e`, build #42404346123](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/actions/runs/42404346123) compiló y su artefacto GitHub #13587033044 estaba disponible hasta el 14-11-2026. `main` móvil `d830ed0` tiene CI aprobada, pero **no existe evidencia física Android/Shelly** de esa versión en esta auditoría. Las incidencias [#42](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/issues/42), [#52](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/issues/52) y [#53](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/issues/53) continúan abiertas; el [gate Production Release Readiness](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/actions/runs/42404346141) falló de manera esperada. **No marcar pruebas físicas como PASS ni considerar pairing Shelly productivo.**
