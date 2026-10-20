# Release notes — sets-frontend-architecture 1.4.1 → 1.5.0

## Objetivo

Alinear el programa con **SETS Framework v1.4.0 / Conceptual Mastery**, manteniendo su identidad específica de arquitectura frontend.

## Cambios principales

- Programa actualizado a v1.5.0 y framework a v1.4.0.
- `CONCEPTUAL_ENGINE.md` incorporado como fuente esencial del setup.
- Las cinco lentes conceptuales son adaptativas, no una secuencia obligatoria ni una escala.
- `PROJECT_CONFIG.yaml` define una ruta conceptual-first, stack neutral, laboratorios optativos y un mapa conceptual opcional.
- `PROJECT_RULES.md` desarrolla causalidad, invariantes, límites, contraejemplos, evidencia de medición y fronteras del dominio frontend.
- `CURRICULUM.md` conserva el namespace `F00–F14` y explicita preguntas conceptuales y evidencias posibles.
- `CASEBOOK.md` mejora el caso conductor con estado de interfaz, reintentos, performance, accesibilidad, seguridad y gobernanza.
- Estado inicial limpio; no se migra ni se inventa evidencia.

## Contratos preservados

- Namespace de competencias `F00–F14`.
- Evaluación 0–4 y niveles de ayuda H0–H4; las cinco lentes no son una escala nueva.
- `/close` genera `LAST_HANDOFF.md`, `LEARNING_STATE.md` completo y delta de `EVIDENCE_LOG.md`.
- `CONCEPT_MAP.md` es opcional y no demuestra dominio por sí solo.
- La sincronización GitHub ↔ ChatGPT es manual salvo integración verificada.

## Instalación en un repositorio nuevo

Este release incluye el **repositorio completo**, listo para subir a un GitHub nuevo. No es un patch. Crea `sets-frontend-architecture`, sube todos los archivos manteniendo las rutas y sigue `SETUP_CHATGPT.md`.

## Si ya existiera un repositorio anterior

Conserva el historial Git y revisa diferencias antes de reemplazar archivos. No borres un estado de aprendizaje real ni copies evidencia de otra especialidad. En el Proyecto de ChatGPT, reemplaza las instrucciones activas y las fuentes antiguas por las de este release y `sets-framework` v1.4.0.

## Validación

Los checks automáticos de integridad, YAML y referencias se ejecutan al empaquetar. Las comprobaciones de interacción en `docs/ACCEPTANCE_CHECKS.md` son manuales y quedan pendientes hasta que alguien las ejecute.
