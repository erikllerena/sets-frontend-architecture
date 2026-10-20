# Mapa de competencias — Frontend Architecture & Design

**Programa v1.5.1 · SETS Framework v1.4.1 · Namespace `F00–F14`**

El foco es la arquitectura y el comportamiento del cliente web. API/BFF, backend y plataforma aparecen como fronteras de contrato, latencia, seguridad, fallos y entrega, no como cursos de otras disciplinas.

Este mapa define competencias prioritarias, no agota todos los temas que pueden estudiarse. SETS puede enseñar una pregunta frontend pertinente fuera de `F00–F14` y relacionarla con una competencia existente cuando ayude; solo se propone un módulo nuevo si el tema es recurrente o estratégicamente central. Fundamento, profundización y especialización son alcances adaptativos, no fases obligatorias. La apertura no cambia el foco frontend.

## Competencias observables

| ID | Módulo | Pregunta conceptual central | Evidencia posible |
|---|---|---|---|
| F00 | Diagnóstico frontend | ¿Qué restricciones del producto, navegador, usuario, equipo y entorno determinan el problema? | Análisis inicial con supuestos, atributos de calidad y riesgos priorizados. |
| F01 | Plataforma web y browser internals | ¿Cómo interactúan networking, event loop, DOM/CSSOM, layout, paint, compositing y caché para producir lo visible? | Traza causal de un comportamiento o degradación, con límites del modelo. |
| F02 | Rendering y entrega | ¿Qué cambia entre MPA, SPA, CSR, SSR, SSG, streaming e hidratación, y qué coste se desplaza a cada fase? | Decisión condicionada por SEO, latencia, interactividad, personalización y operación. |
| F03 | Modularidad y componentes | ¿Qué responsabilidad debe cambiar junta y qué dependencia conviene hacer explícita? | Mapa de módulos/componentes, contratos y plan de refactor argumentado. |
| F04 | Estado y datos del cliente | ¿Cómo se origina, actualiza, invalida y reconcilia el estado de UI, remoto, caché y estado derivado? | Tabla de estados y transiciones que contempla errores, concurrencia y navegación. |
| F05 | Integración con API/BFF | ¿Cómo afecta la incertidumbre de red al contrato, autenticación, errores, reintentos y experiencia de usuario? | Flujo cliente–API/BFF con estados de carga/error, contratos y comportamiento ante timeout. |
| F06 | Microfrontend architecture | ¿Qué problema organizativo/técnico resolvería la separación y qué nuevos costes de runtime, integración y UX introduce? | Comparación entre monolito modular, monorepo, paquetes y MFE con criterios explícitos. |
| F07 | Web performance | ¿Qué parte del tiempo de usuario se está consumiendo y qué evidencia distingue causa de correlación? | Hipótesis, método reproducible, presupuesto y resultados medidos o plan de medición etiquetado. |
| F08 | Seguridad frontend | ¿Qué fronteras de confianza existen en el navegador y cómo podrían explotarse o mitigarse? | Threat model contextual con XSS, CSRF, CSP, dependencias, tokens y límites de cada defensa. |
| F09 | Design systems y accesibilidad | ¿Cómo se preservan semántica, teclado, foco, contraste y consistencia a través de componentes y equipos? | Evaluación accesible con criterios verificables y plan de adopción/gobernanza. |
| F10 | Testing y calidad frontend | ¿Qué riesgo reduce cada nivel de prueba y qué fallos quedan fuera de su cobertura? | Estrategia de pruebas de componentes, integración, E2E, accesibilidad, visual y contratos. |
| F11 | Build, delivery y CDN | ¿Cómo se transforman y publican los artefactos, y qué implica cachear, versionar o revertir una entrega? | Flujo de build/deploy con invalidación, compatibilidad, rollback y supuestos. |
| F12 | Observabilidad del cliente | ¿Qué señales revelan errores reales y degradación de UX sin confundir volumen, impacto y causa? | Diseño de RUM/error reporting, segmentación, alertas accionables y límites de privacidad. |
| F13 | Arquitectura multi-equipo y gobernanza | ¿Cómo se distribuyen ownership, contratos, dependencias y cambios sin crear coordinación excesiva? | Política de versionado, ownership y migración con costes de coordinación explícitos. |
| F14 | Capstone frontend | ¿Qué diseño satisface las necesidades actuales y puede evolucionar sin pagar complejidad injustificada? | Dossier de arquitectura, decisiones defendidas, riesgos, medición y validación selectiva. |

## Método de aprendizaje

1. Diagnóstico adaptativo, una pregunta significativa por turno; no sustituye la enseñanza.
2. Tras el diagnóstico, resumir brechas observadas, proponer una ruta provisional e iniciar una lección conceptual.
3. Aplicar las lentes de `CONCEPTUAL_ENGINE.md` según lo necesite el concepto: origen, mecanismo, límites, alternativas y transferencia. No son pasos obligatorios ni niveles de dominio.
4. Explicar el mecanismo antes de elegir framework, patrón o librería. Distinguir principios de implementación.
5. Proponer práctica optativa con un objetivo claro. No iniciar un laboratorio automáticamente ni exigir código cuando un diagrama, tabla de estados o análisis causal sea mejor.
6. Evaluar por evidencias observables, nivel de ayuda y transferencia novedosa; no por experiencia declarada ni lectura pasiva.
7. La ruta es adaptativa: no es necesario terminar todos los módulos antes de abordar un problema real.

## Rutas posibles

- **Fundamentos de plataforma:** F01 → F02 → F04/F07, adaptado a las brechas.
- **Arquitectura de aplicación:** F03 → F04 → F05 → F10/F11.
- **Frontend de producto confiable:** F02 → F04/F05 → F07/F08/F09/F10/F12.
- **Plataforma multi-equipo:** F03 → F06 → F11/F12/F13 → F14.

Estas rutas son orientativas, no prerrequisitos rígidos.

## Selección de tecnologías

El principio y el mecanismo van primero; después se elige la representación más clara. React y Angular son puentes posibles, no requisitos. Compararlos cuando sus diferencias de reactividad, rendering, composición, estado o DI expliquen una decisión. También puede usarse JavaScript nativo, HTML/CSS, un diagrama o pseudocódigo.
