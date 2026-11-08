# SmartHome — control de cierre documental y aceptación

**SENA ADSO 3145555 · Corte de verificación: 7 de noviembre de 2026**

**Objeto:** permitir que el instructor revise el contenido ya presentado, identifique pendientes reales y no confunda un PR documental con el cierre técnico de la aplicación. Esta lista no acredita autorizaciones personales ni aprueba software en producción.

## 1. Entrega documental en la rama del PR #17

**PR institucional:** https://github.com/code-sena/ADSO-3145555/pull/17 — **ABIERTO / NO FUSIONADO** al momento de esta verificación.

| Sección | Evidencia en el PR #17 | Estado |
|---|---|---|
| 01 Requisitos | `01-requirements-specification/requirements-specification.pdf` | Presente, pendiente de revisión |
| 02 Análisis | `02-software-analysis/02-software-analysis.pdf` | Presente, pendiente de revisión |
| 03 Propuesta técnica | `03-technical-proposal/03-technical-proposal.pdf` y DOCX | Presente, pendiente de revisión |
| 04 Diseño | `04-software-design/04-software-design.pdf` | Presente, pendiente de revisión |
| 05 Pruebas | `05-test-documentation/05-test-documentation.pdf`, protocolo QA Android/Shelly en PDF y MD, matriz CSV de 18 casos | Documentado; **pruebas físicas pendientes** |
| 06 Implementación | `06-implementation-procedure/06-implementation-procedure.pdf` | Presente, pendiente de revisión |
| 07 Acciones de mejora | `07-improvement-actions/07-improvement-actions.pdf` y DOCX | Presente, pendiente de revisión |
| 08 Manuales | `08-manuals/technical-manual.pdf`, `installation-manual.pdf`, `end-user-manual.pdf`; DOCX y MD | Tres manuales presentes, pendiente de revisión |
| 09 Artículo | `09-project-article/09-project-article.pdf` | Presente, pendiente de revisión |

**No están fusionados a `code-sena/main`**; ver el índice `DOCUMENTACION-DEL-RELEASE.md` para abrir los archivos desde la rama PR. No declarar aprobación académica hasta revisión del instructor.

## 2. Pendientes priorizados — acciones concretas

| Prioridad | Bloqueo | Responsable de actuación | Evidencia que debe dejarse |
|---|---|---|---|
| P0 | **Consentimiento de publicación de datos personales** aún sin marcar 3/3. Los archivos públicos de trabajo contienen números de identificación precargados; revisión urgente con los titulares e instructor antes de aprobación | Cada integrante; instructor líder | Autorización válida o decisión documentada sobre divulgación/redacción. **No marcar casillas en nombre de nadie** |
| P0 | PR duplicado [#13](https://github.com/code-sena/ADSO-3145555/pull/13) continúa abierto; sus cinco archivos ya fueron incorporados al #17 | Autora de #13 | Verificar contenido y cerrar #13 **sin fusionar** |
| P0 | Fusionar PR único [#17](https://github.com/code-sena/ADSO-3145555/pull/17) una vez revisado | Mantenedor `code-sena` / instructor | Revisión formal, merge aprobado y enlace a `main` |
| P1 | Videos sección 10: propuestas **pitch 01:30** y **tutorial 04:45** en Drive **privado**. Se detectaron posibles datos identificables; copias locales con ocultaciones no sustituyen los enlaces actuales | Equipo audiovisual y titulares | Revisión integral del video/audio, aprobación, versiones definitivas seguras, permiso público **Lector** y prueba en incógnito |
| P1 | Cinco tags `final-delivery-2026` y **diez ZIP de código** no creados/adjuntados. Release del fork [`final-delivery`](https://github.com/Kevin-Stiven-Lopez-Amaya404/ADSO-3145555/releases/tag/final-delivery) solo tiene `SmartHome.zip` documental | Dueños de cinco repositorios + responsable QA/release | SHAs de `main` aprobados, tags anotados, snapshots y espejos Git completos, 10 SHA-256 reales, 10 Assets con enlaces |
| P1 | Divergencia de repos históricos y canónicos: `smart-home-docs` vs `smart-home-doc`, `smart-home-database` vs `smarthome-database` | Instructor/equipo | Decisión expresa sobre si los actuales se añaden como sexto/séptimo paquete; no sustituir los cinco exigidos |
| P1 | Permiso **Write** para instructor `ariel5253` en cinco repos | Propietarios | Captura/confirmación de invitación aceptada y rol Write |
| P1 | CI web `main` upstream fallida al arrancar Nginx: alias de backend no resoluble. Corrección [PR #7 del fork](https://github.com/Kevin-Stiven-Lopez-Amaya404/smarthome-frontend-web/pull/7) sí pasó; upstream rechazó crear PR con 403 | Natalia / colaborador con Write | PR a `dev` upstream, CI y promoción con QA a `main`; `WEB-CI-BLOQUEO-Y-HOTFIX-2026-11-07.md` |
| P1 | QA Android/Shelly físico y pairing productivo no demostrados. Issues [#42](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/issues/42), [#52](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/issues/52), [#53](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/issues/53) abiertos | Equipo móvil/QA | Matriz de 18 casos con resultados físicos, evidencia depurada, análisis de 5 moderadas y aprobación; **se deja en pausa por ahora** |
| P2 | Roles y aportes 3/3 y campos jurídicos del registro aún por ratificar | Autores e instructor | `team-roster.md` y `software-registration.md` confirmados, origen, clase de obra, publicación y licencias de terceros |
| P2 | Enlaces de Drive, especialmente materiales finales, sin prueba global de acceso anónimo | Propietarios Drive | Probar enlaces definitivos en ventana privada con permisos de solo lectura |

## 3. Evidencia técnica que ya puede declararse sin exagerar

- Móvil: PR [#61](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/pull/61) Expo SDK 58 y PR [#49](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/pull/49) promoción a `main` figuran **fusionados**. `main` observado: `d830ed08886618491ebba2429fd4ffd615ba75ea`; [Mobile CI](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/actions/runs/42406563397) aprobada.
- APK Android POC: [QA build #42404346123](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/actions/runs/42404346123) sobre `6c3946e970711d1352bf2c8c2a54b0816f3afbe7`; **debug**, no APK de producción ni prueba física exitosa. Se intentó abrir el proyecto mediante **Expo Go**, que no reconoce el esquema de Development Build; esto no es evidencia de fallo de la APK SmartHome, ni de éxito de instalación.
- Auditoría de dependencias realizada localmente en el candidato: `npm audit` general notificó **13 vulnerabilidades** (12 moderadas, 1 alta); `npm audit --omit=dev --audit-level=high` notificó **5 moderadas, 0 altas/críticas** entre las dependencias clasificadas como producción. No ejecutar `npm audit fix --force`, pues propone un downgrade incompatible de Expo. Los hallazgos moderados requieren análisis.
- [Production Release Readiness](https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil/actions/runs/42404346141) **falló de manera esperada**, al mantener abiertos #42, #52 y #53. No interpretar CI verde como autorización de release.

## 4. Condición para declarar entrega completamente terminada

No marcar **ENTREGA FINAL COMPLETA** hasta que: (1) el instructor acepte y fusione el PR único, (2) autorizaciones personales y campos legales estén ratificados, (3) haya enlaces a dos videos aprobados y accesibles sin cuenta, (4) se comprueben permisos Write, y (5) estén los cinco tags y diez ZIP auténticos con sus SHA-256 y revisiones técnicas. Cualquier prueba física en pausa debe informarse claramente como tal.

**Estado actual: DOCUMENTACIÓN PREPARADA PARA REVISIÓN; CIERRE INSTITUCIONAL, LEGAL, AUDIOVISUAL Y TÉCNICO PENDIENTE.**
