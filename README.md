# SETS | Frontend Architecture & Design

**Programa v1.5.2 · SETS Framework v1.4.1**

## Misión

Desarrollar comprensión conceptual profunda, criterio técnico y autonomía para diseñar, evaluar, operar y evolucionar aplicaciones y plataformas frontend web mantenibles, accesibles, seguras y eficientes.

El currículo y el casebook son mapas abiertos, no límites exhaustivos. Las tecnologías familiares son contexto opcional; el tutor puede abordar temas y casos nuevos cuando ayuden, manteniendo el foco de esta disciplina.

**Ámbito propio:** plataforma web y navegador, rendering, modularidad, componentes, estado y datos del cliente, integración con APIs/BFF, microfrontends, performance, seguridad, accesibilidad, testing, entrega, observabilidad y gobernanza multi-equipo.

## Principios

- **Conceptos antes que herramientas:** entender el problema, el mecanismo causal, las invariantes y los límites antes de elegir una librería o framework.
- **Tecnología neutral:** React, Angular, TypeScript, JavaScript, Vue, Svelte y otras tecnologías son ejemplos posibles, no requisitos ni el currículo.
- **Profundidad adaptable:** no reducir la enseñanza a definiciones breves ni convertir cada tema en una secuencia rígida de pasos.
- **Práctica con propósito:** diagramas, trazas, contratos, experimentos, código o análisis son formatos válidos. Los laboratorios son optativos salvo que se pidan.
- **Evidencia honesta:** una explicación del tutor, un ejemplo leído o una prueba no ejecutada no demuestra dominio del estudiante ni rendimiento medido.
- **Autonomía académica:** este programa tiene su propio currículo, estado, evidencias y continuidad. No depende del progreso de otros proyectos SETS.

## Archivos principales

- `CHATGPT_PROJECT_INSTRUCTIONS.md`: instrucciones activas listas para pegar en el Proyecto de ChatGPT.
- `PROJECT_RULES.md`: contrato pedagógico específico de frontend.
- `PROJECT_CONFIG.yaml`: objetivo, preferencias y reglas de interacción.
- `learning/CURRICULUM.md`: competencias `F00–F14`.
- `learning/CASEBOOK.md`: casos progresivos con supuestos explícitos.
- `learning/INTERVIEW_SPRINT.md`: preparación opcional para entrevistas frontend.
- `learning/REFERENCES.md`: fuentes técnicas y documentación.
- `state/LEARNING_STATE.md`, `state/EVIDENCE_LOG.md`: estado inicial limpio y registro de evidencias reales.
- `state/CONCEPT_MAP.md`: mapa conceptual opcional; no es una calificación ni prueba de dominio.
- `docs/ACCEPTANCE_CHECKS.md`: comprobaciones manuales sugeridas, no ejecutadas automáticamente.
- `SETUP_CHATGPT.md`: guía de instalación y configuración.

`state/LAST_HANDOFF.md` no se incluye de forma artificial: se genera al primer cierre real con `/close`.

## Inicio rápido

1. Crea el repositorio GitHub **`sets-frontend-architecture`** con los archivos de este paquete.
2. Crea un Proyecto de ChatGPT llamado **SETS | Frontend Architecture & Design**.
3. Sigue `SETUP_CHATGPT.md`: pega solo `CHATGPT_PROJECT_INSTRUCTIONS.md` en las instrucciones y carga las fuentes indicadas.
4. Empieza con `/start` o entra directamente a un tema con `/learn <tema>`.
5. Al terminar una sesión, usa `/close`, revisa los artefactos propuestos y guarda los cambios manualmente.

No existe sincronización automática GitHub ↔ ChatGPT. No subas secretos, datos sensibles ni código propietario del trabajo.


## Archivos del Proyecto de ChatGPT

Las fuentes se suben **como archivos sueltos**: consulta `SETUP_CHATGPT.md` para distinguir esenciales, recomendadas y bajo demanda. Las guías en `state/`, `labs/` y `decisions/` tienen nombres inequívocos (`STATE_ARTIFACTS_GUIDE.md`, `LAB_GUIDE.md` y `ARCHITECTURE_DECISIONS_GUIDE.md`); los `README.md` raíz quedan en GitHub. El mapa conceptual es recomendado, no obligatorio; los laboratorios y las pruebas del tutor no son fuentes permanentes requeridas.
