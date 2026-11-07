# Auditoría de permisos de Drive — SmartHome
**ADSO 3145555 · Revisión de metadatos realizada el 7 de noviembre de 2026**

## Hallazgo importante
La carpeta original [SmartHome en Drive](https://drive.google.com/drive/folders/1FI2E_qAiMVAG1lDXIPhSyPoFF3Pc8ndQ) y los **15 archivos** encontrados en sus 12 secciones reportaron permiso público `anyone: writer` (Cualquier persona → Editor). Es **demasiado amplio** para la entrega del instructor: terceros con el enlace podrían cambiar los archivos.

También reportaron `anyone: writer` el SRS alternativo `SRS FINAL 2026 (1).docx` y las grabaciones [web](https://drive.google.com/file/d/1tHwTE0U6y-zqq21HLuVf-DWIkSUkGD4H/view) y [Android](https://drive.google.com/file/d/1pvq5EGWSaJiv56x05SOM9AKqc26S-I00/view).

**Se recomienda cambiar todos esos accesos públicos a `Cualquier persona con el enlace → Lector`, manteniendo acceso de edición solo para integrantes específicos.** No se cambió ningún permiso mediante el conector; esta comprobación es de metadatos de Google Drive y no sustituye la prueba anónima del enlace en incógnito.

## Inventario de carpetas y archivos fuente
| Sección | Archivos visibles en Drive | Acceso público observado |
|---|---|---|
| 01 Documentos generales | SRS_SMART_HOME_ACTUALIZADO_2026 (1).md; costos_proyecto_smart_home.xlsx | Editor |
| 02 Navegación | Documento Navegacion Smart Home.docx | Editor |
| 03 Propuesta técnica | CONTENIDO PROPUESTA TECNICA Y ECONOMICA.docx | Editor |
| 04 Diseño | INFORME DE DISEÑO.docx; INFORME DE DISEÑO (1).docx | Editor |
| 05 Artefactos de código / Repo | Repositorio.txt (solo enlace, no copia Git) | Editor |
| 06 Pruebas | Documento Integrado de Manuales Técnico, de Instalación y de Usuario Final (2).docx | Editor |
| 07 Implementación | Documento Integrado de Manuales Técnico, de Instalación y de Usuario Final (2).docx | Editor |
| 08 Acciones de mejora | Acciones Correctivas, Preventivas y de Mejora (1).docx | Editor |
| 09 Manuales | Controles Smart Home ISO2 (1).docx | Editor |
| 10 Artículo | Smart_Home_Articulo_Proyecto.pdf | Editor |
| 11 Despliegue | Documento_Despliegue_Smart_Home_SENA.1.2docx.docx | Editor |
| 12 Términos | Politica_Tratamiento_Datos_Smart_Home.docx; Terminos_y_Condiciones_SMART_HOME.docx | Editor |

**Posible incongruencia documental adicional:** la sección 06 (Pruebas) contiene un documento llamado "Manuales ...", no una matriz de pruebas. Este hecho no acredita que el contenido sea inválido, pero debe comprobarse antes de marcar esa carpeta como cumplida. El PR #17 incluye una documentación de pruebas en PDF distinta.

## Procedimiento de corrección por el propietario
1. Abrir la carpeta de Drive → **Compartir → Acceso general**.
2. Escoger **Cualquier persona con el enlace** y rol **Lector**, nunca Editor.
3. Revisar las carpetas hijas y cada archivo: el acceso explícito `anyone: writer` puede existir independientemente del de la carpeta. Cambiarlo a **Lector** en los documentos originales, SRS alternativo y videos.
4. Probar desde una ventana privada (sin iniciar sesión), al menos el enlace a la carpeta, SRS, pitch y tutorial final. Comprobar que se pueden **abrir pero no editar**.
5. Verificar que los documentos para publicación no contengan secretos, contraseñas, identificaciones no autorizadas ni información personal innecesaria. Mantener las autorizaciones del README pendientes hasta confirmar las tres.
6. Registrar capturas o enlaces de revisión con fecha. No afirmar que todo quedó corregido hasta verificarlo.

**Limitación:** el conector no permite editar el permiso público `anyone` desde esta conversación. La operación corresponde al propietario de Drive.

## Enlaces y trazabilidad
- [Inventario documental](DOCUMENTACION-DEL-RELEASE.md)
- [Videos y estado de duración](10-videos/video-links.md)
- [Respuesta a las 14 correcciones](RESPUESTA-14-CORRECCIONES-INSTRUCTOR.md)
