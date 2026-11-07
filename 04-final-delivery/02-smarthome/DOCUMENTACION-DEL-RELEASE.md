# SmartHome — Inventario de entrega académica
**SENA · ADSO 3145555 · Revisión 7 de noviembre de 2026**

Este inventario consolida en el **PR #17** los archivos originalmente aportados en el PR #13 por Karen Daniela Holguín Cruz y los informes técnicos subidos por Kevin Stiven López Amaya. La incorporación a `code-sena/main` continúa sujeta a aprobación institucional.

## Archivos requeridos y sus PDF

| Sección institucional | PDF final en este PR | Fuente editable o material de apoyo |
|---|---|---|
| 01 Requisitos | [requirements-specification.pdf](01-requirements-specification/requirements-specification.pdf) | [Referencia SRS](01-requirements-specification/source-reference.md), archivo Markdown original en la carpeta Drive |
| 02 Análisis de software | [02-software-analysis.pdf](02-software-analysis/02-software-analysis.pdf) | [Markdown](02-software-analysis/02-software-analysis.md) |
| 03 Propuesta técnica | Pendiente exportar a PDF final | Documento Word original bajo [03](03-technical-proposal/) (procedente del PR #13) |
| 04 Diseño de software | [04-software-design.pdf](04-software-design/04-software-design.pdf) | [Markdown](04-software-design/04-software-design.md), Word original en carpeta Drive |
| 05 Pruebas | [05-test-documentation.pdf](05-test-documentation/05-test-documentation.pdf) | [Markdown](05-test-documentation/05-test-documentation.md) |
| 06 Procedimiento de implementación | [06-implementation-procedure.pdf](06-implementation-procedure/06-implementation-procedure.pdf) | [Markdown](06-implementation-procedure/06-implementation-procedure.md) |
| 07 Acciones correctivas y mejora | Pendiente PDF final | [Markdown](07-improvement-actions/07-improvement-actions.md), Word original del PR #13 |
| 08 Manuales | Pendiente PDF final de manuales | [Manual técnico](08-manuals/technical-manual.md), [instalación](08-manuals/installation-manual.md), [usuario](08-manuals/end-user-manual.md) y documento original del PR #13 |
| 09 Artículo | [09-project-article.pdf](09-project-article/09-project-article.pdf) | [Markdown](09-project-article/09-project-article.md), PDF original del PR #13 |
| 10 Videos | [Videos verificados](10-videos/video-links.md) | Falta un pitch de 1–2 minutos y tutorial de 3–5 minutos conforme a guía |
| code-tag | [Estado de repositorios y tags](code-tag/README.md) | Falta aprobar tags, generar diez ZIP y calcular SHA-256 reales |
| Registro | [Equipo](team-roster.md) · [Registro software](software-registration.md) | Roles y aportes documentados para ratificación; autorizaciones de datos aún sin marcar |

## Archivos originales y paquete opcional para Release

[Carpeta original de Google Drive](https://drive.google.com/drive/folders/1FI2E_qAiMVAG1lDXIPhSyPoFF3Pc8ndQ): contiene 15 archivos en 12 secciones, además de sus duplicados históricos. El paquete local `SmartHome_Release_Todo.zip` combina los 15 originales de Drive con los 37 archivos documentales preparados previamente. **Un ZIP de documentos no sustituye los diez ZIP de código obligatorios.**

## Presentación de un solo PR

- [PR #17](https://github.com/code-sena/ADSO-3145555/pull/17) contiene los cinco archivos del [PR #13](https://github.com/code-sena/ADSO-3145555/pull/13) sin alterar su autoría original. Se solicita a la autora del PR #13 cerrarlo tras validar la consolidación para mantener un único PR activo de SmartHome.
- El [PR #5](https://github.com/code-sena/ADSO-3145555/pull/5) tiene cambios ajenos a este proyecto y no debe integrarse como entrega final.
- La entrega necesita aprobación institucional; los permisos de la cuenta conectada impiden fusionar en `code-sena/main`.

**Estado:** PDF académicos 01/02/04/05/06/09 disponibles; registros técnicos parcialmente diligenciados; videos y tags todavía no conformes.

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
