# Instalación — SETS | Frontend Architecture & Design

## 1. Crea el repositorio y el Proyecto

- Repositorio GitHub sugerido: **`sets-frontend-architecture`**.
- Proyecto de ChatGPT sugerido: **SETS | Frontend Architecture & Design**.
- Si la opción está disponible, utiliza memoria solo del Proyecto para mantener aislado el progreso académico.

Este paquete contiene el repositorio completo para una instalación nueva; no necesitas un repositorio frontend anterior ni archivos de otra especialidad.

## 2. Instrucciones activas

En las instrucciones del Proyecto pega **solo** el contenido de `CHATGPT_PROJECT_INSTRUCTIONS.md`. No concatenes varios documentos extensos: las fuentes adicionales se cargan por separado.

## 3. Fuentes del framework SETS v1.4.1

Desde el repositorio `sets-framework`, carga como fuentes esenciales:
- `core/PROJECT_INSTRUCTIONS.md`
- `core/CONCEPTUAL_ENGINE.md`
- `core/INTERACTION_ENGINE.md`
- `core/DECISION_ENGINE.md`
- `core/PRACTICE_ENGINE.md`
- `core/ASSESSMENT_ENGINE.md`
- `core/SESSION_HANDOFF.md`
- `templates/LAST_HANDOFF.template.md`

Fuentes recomendadas según disponibilidad: `docs/REFERENCE_POLICY.md`, `docs/LEARNING_SCIENCE.md`, `docs/COMMAND_REFERENCE.md` y `templates/ADR_TEMPLATE.md`.

**Importante:** usa los archivos de `sets-framework` v1.4.1, no una copia antigua v1.3.x. La referencia a `CONCEPTUAL_ENGINE.md` es necesaria para la profundidad conceptual de este programa.

## 4. Fuentes de este repositorio

Carga:
- `PROJECT_CONFIG.yaml`
- `PROJECT_RULES.md`
- `learning/CURRICULUM.md`
- `learning/CASEBOOK.md`
- `learning/INTERVIEW_SPRINT.md`
- `learning/REFERENCES.md`
- `state/LEARNING_STATE.md`
- `state/EVIDENCE_LOG.md`
- Opcional: `state/CONCEPT_MAP.md`

`state/LAST_HANDOFF.md` no se adjunta antes del primer `/close` real porque todavía no existe una sesión que documentar.

## 5. Primer uso

- `/start`: diagnóstico breve, una pregunta por turno; después se inicia enseñanza conceptual.
- `/learn <tema>`: lección conceptual adaptada a tu pregunta y nivel demostrado.
- `/deep <tema>`: mecanismos internos, límites y casos de fallo.
- `/design <sistema>` o `/decision <problema>`: comparar opciones con restricciones explícitas.
- `/lab <tema>`: práctica implementable cuando tú la pidas; también puedes elegir análisis sin código.
- `/close`: genera handoff, estado completo y delta de evidencias para que los revises.
- `/resume`: retoma solo desde el estado verificable de este programa.

## 6. GitHub ↔ ChatGPT

La sincronización es manual salvo que una integración real confirme una escritura. Tras `/close`, revisa los tres artefactos, guárdalos en GitHub y actualiza las fuentes del Proyecto. No reemplaces el registro acumulativo de evidencias con un archivo vacío.

## 7. Verificación rápida

Pregunta al Proyecto:
1. «¿Cuál es el ámbito de este programa?»
2. «¿Cómo decides cuándo usar React, Angular u otra tecnología?»
3. «¿Cuándo propones un laboratorio?»
4. «¿Qué archivos deben generarse al usar `/close`?»

Las respuestas deben concordar con `PROJECT_RULES.md` y `docs/ACCEPTANCE_CHECKS.md`. Estas comprobaciones son manuales sugeridas; el paquete no afirma que ya se hayan ejecutado.


## Currículo y casos abiertos (v1.5.1)

Las fuentes de esta versión declaran el currículo y el casebook como mapas no exhaustivos. Al actualizar el Proyecto de ChatGPT, reemplaza las instrucciones activas y las fuentes antiguas por las de este paquete y por SETS Framework v1.4.1. Las pruebas de `docs/ACCEPTANCE_CHECKS.md` son manuales y quedan pendientes hasta ejecutarlas.
