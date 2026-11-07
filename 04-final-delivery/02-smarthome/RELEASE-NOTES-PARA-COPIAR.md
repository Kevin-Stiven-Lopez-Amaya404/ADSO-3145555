# Final Delivery — SmartHome

**Training Program:** Software Analysis and Development (ADSO)  
**Training Group:** 3145555  
**Institution:** Servicio Nacional de Aprendizaje (SENA)  
**Project:** SmartHome — Smart Home Energy Management

## Project Overview

SmartHome is a smart-home platform for managing homes and connected devices, displaying energy consumption and notifications, and communicating with supported devices. The system integrates a NestJS/TypeScript backend, React/Vite web client, React Native/Expo mobile client, and PostgreSQL database with Liquibase. Device communication involves MQTT and experimental Shelly LAN/BLE workflows.

## Source Code Repositories

- Backend: https://github.com/nataliachala1/smarthome-backend
- Web frontend: https://github.com/nataliachala1/smarthome-frontend-web
- Mobile application: https://github.com/Kevin-Stiven-Lopez-Amaya404/from_movil
- Database: https://github.com/nataliachala1/smarthome-database
- Technical documentation: https://github.com/Kevin-Stiven-Lopez-Amaya404/smart-home-doc

## Academic Documentation

The project documentation is organized in the institutional folder:

**[04-final-delivery/02-smarthome/](https://github.com/code-sena/ADSO-3145555/tree/main/04-final-delivery/02-smarthome)**

Included deliverables: software analysis, architecture/design, test documentation, implementation procedure, corrective and improvement actions, technical/installation/end-user manuals, project article, project team and registration records. Requirements specification, technical proposal and two videos are tracked in the corresponding folder and must be confirmed before submission.

An optional supporting asset, `SmartHome_Documentacion_Release_ADSO-3145555.zip`, contains the prepared PDF, Word and Markdown documents. This **does not replace** the institutional documentation folder.

## Code Packages and Integrity

For each approved **original code repository**, publish both:

- `<repo>-final-delivery-2026-main.zip` — snapshot of the approved `main` commit carrying annotated tag `final-delivery-2026`.
- `<repo>-full-export.zip` — full Git history including branches and tags.

Publish the files as **Release Assets** in this fork. Record their real SHA-256 checksums and download links in **[code-tag/SHA256SUMS.txt](https://github.com/code-sena/ADSO-3145555/tree/main/04-final-delivery/02-smarthome/code-tag/SHA256SUMS.txt)**. Do not invent checksum strings or attach a nonvalidated branch as the final code snapshot.

## Acceptance Status

**At document preparation (7 November 2026):** the web `main` CI smoke test had failed; mobile security PR #61 and QA-to-main PR #49 remained draft/open and physical Android acceptance was pending. This Release **must remain unpublished as a final verified code delivery** until the build, acceptance and tags are completed. The academic documentation can be reviewed independently.

## Project Team

- Natalia Chala Chala
- Kevin Stiven López Amaya
- Karen Daniela Holguín Cruz
