# SmartHome

Final delivery of the training project / Entrega final del proyecto formativo.

## General information / Información general

| Field / Campo | Value / Valor |
|---|---|
| Product name / Nombre del producto | SmartHome |
| Ficha | 3145555 |
| Training program / Programa de formación | Análisis y Desarrollo de Software (228118) |
| Training project / Proyecto formativo | Desarrollo de software orientado a servicios |
| Training center / Centro de formación | Centro de la Industria, la Empresa y los Servicios (Regional Huila) |
| Process / Proceso | Completion of the technologist taught stage / Finalización de la etapa lectiva del tecnólogo |
| Research seedbed / Semillero de investigación | Developers & Geeks |
| Delivery version / Versión entregada | Objetivo `final-delivery-2026`; tags de código pendientes de aprobación/publicación |
| Delivery date / Fecha de entrega | 2026-11-07 (Release documental publicado; entrega técnica pendiente de aceptación) |
| Delivered by / Entregado por | Kevin Stiven López Amaya (fork de entrega) |

## Summary / Resumen

- *Problem it solves / Problema que resuelve:* Facilita la gestión de hogares y dispositivos conectados, el control de dispositivos compatibles y la consulta del consumo eléctrico.

- *Target users / Usuarios:* Usuarios que necesitan gestionar hogares y dispositivos conectados. El perfil específico de usuario está pendiente de validación.

- *Main features / Funciones principales:*
  - Autenticación, activación de cuentas y recuperación de contraseñas.
  - Gestión de hogares, invitaciones y membresías.
  - Gestión de dispositivos y órdenes de encendido y apagado.
  - Consulta de consumo eléctrico.
  - Comunicación mediante MQTT y Socket.IO.
  - API de notificaciones.

- *Technology stack / Tecnologías:*
  - Backend: NestJS 11, TypeScript, Prisma 7 y Node.js.
  - Frontend web: React 18, TypeScript y Vite 6.
  - Aplicación móvil: React Native, Expo 57 y TypeScript.
  - Base de datos: PostgreSQL.
  - Comunicación: MQTT y Socket.IO.
  - Gestión de migraciones: Liquibase.

- *Production URL / URL en producción:* Pendiente de confirmar.

- *Demo credentials / Credenciales de prueba:* Pendiente de confirmar. No publicar contraseñas reales.
## Team members / Integrantes

> Names and document numbers were preloaded by the instructor from the Sofía Plus report. Each member checks their row, completes GitHub user and role, and marks the last column. Report any error, missing member or extra member to the instructor.
>
> Los nombres y documentos los precargó el instructor desde el reporte de Sofía Plus. Cada integrante revisa su fila, completa usuario de GitHub y rol, y marca la última columna. Reporte al instructor cualquier error, o si falta o sobra alguien.

| Full name / Nombre completo | Doc. type / Tipo | Doc. number / Número | Ficha | GitHub user / Usuario | Role / Rol | Verified and authorized / Verificado y autorizado |
|---|---|---|---|---|---|---|
| KAREN DANIELA HOLGUIN CRUZ | CC | 1079176743 | 3145555 | Karendaniela09 | PostgreSQL/Liquibase y documentación (por ratificar) | ☐ |
| NATALIA CHALA CHALA | CC | 1075508373 | 3145555 | nataliachala1 | Infraestructura y despliegue Docker (por ratificar) | ☐ |
| KEVIN STIVEN LOPEZ AMAYA | CC | 1077724241 | 3145555 | Kevin-Stiven-Lopez-Amaya404 | Backend NestJS/MQTT y documentación técnica (por ratificar) | ☐ |

Data use authorization: by checking the box, the member confirms their data and authorizes publishing their name, document number and ficha in this public repository, for the software registration process (Ley 1581 de 2012). Anyone who does not authorize it tells the instructor before delivering.

Autorización de datos: al marcar la casilla, el integrante confirma sus datos y autoriza publicar su nombre, número de documento y ficha en este repositorio público, para el trámite de registro de software (Ley 1581 de 2012). Quien no lo autorice se lo informa al instructor antes de entregar.

## Delivery contents / Contenido de la entrega

| Folder / Carpeta | Content / Contenido | Done / Listo |
|---|---|---|
| [`01-requirements-specification/`](01-requirements-specification/) | Requirements specification / Especificación de requisitos | PDF del SRS subido en PR #17; pendiente aprobación |
| [`02-software-analysis/`](02-software-analysis/) | Software analysis / Análisis del software | PDF de análisis subido en PR #17; pendiente aprobación |
| [`03-technical-proposal/`](03-technical-proposal/) | Technical proposal / Propuesta técnica | ☐ |
| [`04-software-design/`](04-software-design/) | Software design / Diseño del software | PDF de diseño subido en PR #17; pendiente aprobación |
| [`05-test-documentation/`](05-test-documentation/) | Test documentation / Documentación de pruebas | PDF de pruebas subido en PR #17; pendiente aprobación |
| [`06-implementation-procedure/`](06-implementation-procedure/) | Implementation procedure / Procedimiento de implementación | PDF de implementación subido en PR #17; pendiente aprobación |
| [`07-improvement-actions/`](07-improvement-actions/) | Improvement actions / Acciones de mejoramiento | ☐ |
| [`08-manuals/`](08-manuals/) | Manuals / Manuales | ☐ |
| [`09-project-article/`](09-project-article/) | Project article / Artículo del proyecto | PDF de artículo subido en PR #17; pendiente aprobación |
| [`10-videos/`](10-videos/) | Videos / Videos | ☐ |
| [`code-tag/`](code-tag/) | Repository links, tags and ZIP files / Enlaces, tags y ZIP | ☐ |
| [`team-roster.md`](team-roster.md) | Team and roles / Equipo y roles | ☐ |
| [`software-registration.md`](software-registration.md) | Software registration data / Datos para registro de software | ☐ |

## Large files on Google Drive / Archivos pesados en Google Drive

Only files too heavy for GitHub go here, such as demo videos. Everything else stays in this folder.

Aquí solo van archivos demasiado pesados para GitHub, como videos de demostración. Todo lo demás vive en esta carpeta.

| File / Archivo | Size / Tamaño | Link / Enlace |
|---|---|---|
| | | |

## Autorizaciones y entrega técnica pendientes

Las casillas «Verificado y autorizado» de los tres integrantes **siguen desmarcadas**. Cada persona debe autorizar individualmente la publicación de sus datos y verificar los roles antes de aprobar el registro. No se ha marcado consentimiento en nombre de terceros.

Los PDF académicos de las secciones 01, 02, 04, 05, 06 y 09 están incorporados a la rama del PR #17. Los tags/ZIP de código requieren aprobación y generación verificable; la documentación no sustituye los artefactos del software.

Carpeta de fuentes documentales: https://drive.google.com/drive/folders/1FI2E_qAiMVAG1lDXIPhSyPoFF3Pc8ndQ

## Control actual del Release y los PR

- **[Release documental publicado](https://github.com/Kevin-Stiven-Lopez-Amaya404/ADSO-3145555/releases/tag/final-delivery):** tag del fork `final-delivery`, actualmente con un único Asset `SmartHome.zip` (documentación). **Aún faltan los diez ZIP de código y SHA-256 reales** que exige el instructor; el tag del fork no sustituye los tags anotados `final-delivery-2026` en los repositorios originales.
- **[PR #17](https://github.com/code-sena/ADSO-3145555/pull/17):** entrega documental consolidada para revisión; todavía requiere aprobación institucional.
- **[PR #13](https://github.com/code-sena/ADSO-3145555/pull/13):** aportes incorporados al #17; pendiente de que Daniela verifique y cierre su PR sin fusionarlo.
- **[PR #5](https://github.com/code-sena/ADSO-3145555/pull/5):** cerrado sin fusionar porque sus 546 archivos pertenecían a carpetas ajenas al alcance final de SmartHome.
- **[Auditoría de permisos Drive](AUDITORIA-ACCESO-DRIVE.md):** carpeta y archivos fuente con `anyone: writer`; cambiar a `Cualquier persona con el enlace → Lector` y probar anónimamente.
- **[Respuesta a las 14 correcciones](RESPUESTA-14-CORRECCIONES-INSTRUCTOR.md):** separa lo preparado de lo que requiere aceptación o acción del propietario.
