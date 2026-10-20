# SETS — CONCEPT_MAP | Frontend Architecture & Design

> Mapa conceptual opcional. No es una escala, una fuente paralela de calificaciones ni evidencia de dominio. Las relaciones iniciales son hipótesis de organización que deben revisarse al estudiar los conceptos.

- **Disciplina:** Frontend Architecture & Design
- **Fecha última revisión:** 2026-10-19
- **Foco activo:** relación entre navegador, rendering, estado del cliente, rendimiento y experiencia observable
- **Estado de elaboración:** Inicial

## Conceptos relevantes

| ID | Concepto | Pregunta que ayuda a resolver | Notas / límites del modelo | Evidencia vinculada |
|---|---|---|---|---|
| C-001 | Pipeline de rendering del navegador | ¿Qué trabajo ocurre entre recibir recursos y mostrar una interfaz utilizable? | El diagrama simplifica un pipeline que puede variar por navegador, ruta de código y optimizaciones. | — |
| C-002 | Estado de UI y estado remoto | ¿Qué dato vive en la interfaz y cuál depende de una fuente externa? | La distinción es conceptual; el almacenamiento concreto puede combinarse según el diseño. | — |
| C-003 | Límites de componentes y módulos | ¿Qué debería cambiar junto y qué dependencias deben ser explícitas? | La granularidad óptima depende del dominio, equipo, reutilización y coste de coordinación. | — |
| C-004 | Performance percibida y medida | ¿Qué parte de la experiencia es lenta y qué dato permite localizar la causa? | Una métrica agregada puede ocultar dispositivos, rutas, redes o segmentos afectados. | — |
| C-005 | Accesibilidad y semántica | ¿Puede la misma función descubrirse y utilizarse con distintas capacidades e interfaces de entrada? | Una comprobación automática no demuestra accesibilidad completa. | — |

## Relaciones conceptuales iniciales

| Desde | Relación | Hacia | Justificación causal o criterio | Estado |
|---|---|---|---|---|
| C-001 | mecanismo | C-004 | El trabajo de red, ejecución y rendering puede contribuir a la latencia observada, pero hay que medir para atribuir una causa concreta. | hipótesis |
| C-002 | mecanismo | C-004 | Actualizaciones de estado pueden disparar trabajo de render o peticiones adicionales; el efecto depende del sistema. | hipótesis |
| C-003 | depende_de_contexto | C-004 | Límites y dependencias pueden afectar carga, tamaño del bundle y trabajo en runtime, pero no de forma automática. | hipótesis |
| C-005 | contraste | C-004 | Una optimización de velocidad no garantiza que la interfaz sea comprensible ni operable con teclado o lector de pantalla. | por explorar |

## Preguntas abiertas

- ¿Qué señales permiten distinguir descarga, ejecución de JavaScript, trabajo de layout y coste de rendering?
- ¿Cuándo una fuente de verdad única simplifica la consistencia y cuándo una caché cliente aporta un coste de sincronización excesivo?
- ¿Qué parte de la accesibilidad puede automatizarse y qué requiere revisión manual?

## Mantenimiento

Actualizar solo cuando una relación conceptual justificada ayude a comprender o transferir ideas. El mapa no reemplaza `LEARNING_STATE.md` ni `EVIDENCE_LOG.md`, y no debe añadirse como cuarto artefacto obligatorio de `/close`.
