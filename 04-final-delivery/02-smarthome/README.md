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
  - Aplicación móvil: React Native, Expo y TypeScript. `dev/package.json` consultado el 07-11-2026 declara Expo ~58.0.23 y React Native 0.88.1; el README de `dev` todavía describe Expo 57. La versión final depende del commit y build aprobados.
  - Base de datos: PostgreSQL.
  - Comunicación: MQTT y Socket.IO.
  - Gestión de migraciones: Liquibase.

- *Production URL / URL en producción:* Pendiente de confirmar.

- *Demo credentials / Credenciales de prueba:* Pendiente de confirmar. No publicar contraseñas reales.
## Team members / Integrantes

> Names and document types were preloaded from the instructor's roster. Full identification numbers are withheld from this public version pending individual authorization and should be supplied only via the instructor's private registration channel. Each member must verify their row, GitHub account and role.
>
> Los nombres y tipos de documento proceden de la plantilla del instructor. Los números completos se reservan en esta versión pública hasta confirmar autorización individual y deben entregarse por el canal privado del registro. Cada integrante verifica su fila, usuario de GitHub y rol, y reporta errores al instructor.

| Full name / Nombre completo | Doc. type / Tipo | Doc. number / Número | Ficha | GitHub user / Usuario | Role / Rol | Verified and authorized / Verificado y autorizado |
|---|---|---|---|---|---|---|
| KAREN DANIELA HOLGUIN CRUZ | CC | Reservado — canal privado | 3145555 | Karendaniela09 | PostgreSQL/Liquibase y documentación (por ratificar) | ☐ |
| NATALIA CHALA CHALA | CC | Reservado — canal privado | 3145555 | nataliachala1 | Infraestructura y despliegue Docker (por ratificar) | ☐ |
| KEVIN STIVEN LOPEZ AMAYA | CC | Reservado — canal privado | 3145555 | Kevin-Stiven-Lopez-Amaya404 | Backend NestJS/MQTT y documentación técnica (por ratificar) | ☐ |

Privacy and data verification: the unchecked boxes do not constitute consent. Full identification numbers are not to be included in the public README; the official registration form, if applicable, is completed through an authorized private channel. Refer to the privacy protocol linked below.

Verificación de datos: las casillas sin marcar no implican autorización. Los números completos de identificación no se incluyen en este README público; los datos necesarios para el trámite oficial se entregan por un canal privado autorizado. Consultar el protocolo de privacidad enlazado abajo.

## Delivery contents / Contenido de la entrega

| Folder / Carpeta | Content / Contenido | Done / Listo |
|---|---|---|
| [`01-requirements-specification/`](01-requirements-specification/) | Requirements specification / Especificación de requisitos | PDF del SRS subido en PR #17; pendiente aprobación |
| [`02-software-analysis/`](02-software-analysis/) | Software analysis / Análisis del software | PDF de análisis subido en PR #17; pendiente aprobación |
| [`03-technical-proposal/`](03-technical-proposal/) | Technical proposal / Propuesta técnica | [PDF](03-technical-proposal/03-technical-proposal.pdf) y [Word editable](03-technical-proposal/03-technical-proposal.docx) incorporados al PR; aprobación pendiente |
| [`04-software-design/`](04-software-design/) | Software design / Diseño del software | PDF de diseño subido en PR #17; pendiente aprobación |
| [`05-test-documentation/`](05-test-documentation/) | Test documentation / Documentación de pruebas | PDF de pruebas subido en PR #17; pendiente aprobación |
| [`06-implementation-procedure/`](06-implementation-procedure/) | Implementation procedure / Procedimiento de implementación | PDF de implementación subido en PR #17; pendiente aprobación |
| [`07-improvement-actions/`](07-improvement-actions/) | Improvement actions / Acciones de mejoramiento | [PDF](07-improvement-actions/07-improvement-actions.pdf), [Word](07-improvement-actions/07-improvement-actions.docx) y Markdown actualizados en PR; aprobación pendiente |
| [`08-manuals/`](08-manuals/) | Manuals / Manuales | [Técnico](08-manuals/technical-manual.pdf), [Instalación](08-manuals/installation-manual.pdf), [Usuario](08-manuals/end-user-manual.pdf), con DOCX y MD; aprobación pendiente |
| [`09-project-article/`](09-project-article/) | Project article / Artículo del proyecto | PDF de artículo subido en PR #17; pendiente aprobación |
| [`10-videos/`](10-videos/) | Videos / Videos | Propuestas privadas pitch 01:30 y tutorial 04:45; revisión de privacidad/audio, aprobación y acceso Lector pendientes |
| [`code-tag/`](code-tag/) | Repository links, tags and ZIP files / Enlaces, tags y ZIP | Auditoría preparada; 5 tags y 10 ZIP técnicos pendientes |
| [`team-roster.md`](team-roster.md) | Team and roles / Equipo y roles | Roles propuestos, pendientes de ratificación individual |
| [`software-registration.md`](software-registration.md) | Software registration data / Datos para registro de software | Campos técnicos propuestos; autoría, consentimientos y declaraciones legales pendientes |

## Large files on Google Drive / Archivos pesados en Google Drive

Only files too heavy for GitHub go here, such as demo videos. Everything else stays in this folder.

Aquí solo van archivos demasiado pesados para GitHub, como videos de demostración. Todo lo demás vive en esta carpeta.

| File / Archivo | Size / Tamaño | Link / Enlace |
|---|---|---|
| | | |

## Autorizaciones y entrega técnica pendientes

Las casillas «Verificado y autorizado» de los tres integrantes **siguen desmarcadas**. Cada persona debe autorizar individualmente la publicación de sus datos y verificar los roles antes de aprobar el registro. No se ha marcado consentimiento en nombre de terceros.

Los PDF académicos de las secciones 01–09, incluido el grupo de tres manuales de 08, están incorporados a la rama del PR #17 (no a la rama institucional `main`). El Word histórico ISO permanece como anexo, sin considerarse un manual independiente. Los tags/ZIP de código requieren aprobación y generación verificable; la documentación no sustituye los artefactos del software.

Carpeta de fuentes documentales: https://drive.google.com/drive/folders/1FI2E_qAiMVAG1lDXIPhSyPoFF3Pc8ndQ

## Control actual del Release y los PR

- **[Release documental publicado](https://github.com/Kevin-Stiven-Lopez-Amaya404/ADSO-3145555/releases/tag/final-delivery):** tag del fork `final-delivery`, actualmente con un único Asset `SmartHome.zip` (documentación). **Aún faltan los diez ZIP de código y SHA-256 reales** que exige el instructor; el tag del fork no sustituye los tags anotados `final-delivery-2026` en los repositorios originales.
- **[PR #17](https://github.com/code-sena/ADSO-3145555/pull/17):** entrega documental consolidada para revisión; todavía requiere aprobación institucional.
- **[PR #13](https://github.com/code-sena/ADSO-3145555/pull/13):** aportes incorporados al #17; pendiente de que Daniela verifique y cierre su PR sin fusionarlo.
- **[PR #5](https://github.com/code-sena/ADSO-3145555/pull/5):** cerrado sin fusionar porque sus 546 archivos pertenecían a carpetas ajenas al alcance final de SmartHome.
- **[Auditoría de permisos Drive](AUDITORIA-ACCESO-DRIVE.md):** revisar en privado los accesos; configurar `Cualquier persona con el enlace → Lector` y probar anónimamente.
- **[Respuesta a las 14 correcciones](RESPUESTA-14-CORRECCIONES-INSTRUCTOR.md):** separa lo preparado de lo que requiere aceptación o acción del propietario.


## Handoff de cierre al instructor — estado actualizado

Ver [control de cierre y aceptación](CIERRE-DOCUMENTAL-Y-ACEPTACION-2026-11-07.md). El PR #17 contiene los PDF de las secciones 01–09 (incluidos 3 manuales de 08) y evidencia QA documental; **no se ha fusionado**, y el PR #13 continúa abierto para cierre sin merge por su autora. El móvil tiene Expo SDK 58 integrado en `main` y CI automatizada aprobada, pero pruebas físicas Android/Shelly y autorización de producción pendientes. El Release conserva un único ZIP documental; cinco tags y diez ZIP de código siguen pendientes. **Antes de publicar o fusionar**, el instructor y cada integrante deben revisar las autorizaciones no marcadas y la presencia de números de identificación precargados en documentación pública; no se considera otorgado consentimiento por defecto.


**Protección de datos para revisión del instructor:** [protocolo de privacidad, consentimientos y registro](PROTOCOLO-PRIVACIDAD-Y-AUTORIZACIONES-2026-11-07.md). Los números de identificación se reservaron en esta versión pública; ello **no elimina** versiones anteriores de Git ni corrige automáticamente otras copias existentes. Revisar con los titulares antes de fusionar.
