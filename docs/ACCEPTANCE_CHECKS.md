# Acceptance checks — Frontend Architecture & Design v1.5.2

Estas comprobaciones son **pruebas manuales sugeridas**; no representan evidencia de que el tutor ya las haya superado.

1. `/start`: una pregunta diagnóstica por turno; al terminar, síntesis breve e inicio de enseñanza conceptual, sin laboratorio automático.
2. `/learn rendering`: explicar problema, mecanismo, supuestos, al menos un límite relevante y alternativa según el contexto.
3. `/deep estado del cliente`: diferenciar UI state, server state, caché y estado derivado antes de elegir librerías.
4. «Explícamelo sin código»: conservar profundidad causal sin imponer implementación.
5. «Elige tú el stack»: escoger una representación o tecnología por valor pedagógico y explicar brevemente el motivo.
6. «Compara React y Angular»: primero mostrar principios compartidos; explicar diferencias de modelo solo cuando ayuden a la decisión.
7. Caso de performance: separar hipótesis, condiciones de medición, métricas y resultados realmente observados.
8. Caso de microfrontends: comparar alternativas modulares y no asumir que MFE es la opción predeterminada.
9. Seguridad/accesibilidad: tratar riesgos y criterios verificables como parte del diseño, no como checklist superficial.
10. Después del diagnóstico, `/lab` no se inicia sin petición o aceptación del estudiante.
11. `/status` en estado inicial: competencias «No evaluado», sin inferir dominio por experiencia declarada.
12. `/close`: tres artefactos obligatorios, sin inventar evidencias; el mapa conceptual sigue siendo opcional.
13. `/resume`: usa solo el estado de este programa, evita duplicar evidencias y declara archivos ausentes o inconsistentes.
14. No se afirma sincronización automática ni guardado en GitHub/Proyecto sin operación comprobada.

## Checks de apertura y foco

- **OL1:** Pedir un ejemplo con una tecnología no incluida en la lista familiar: el tutor puede usarla si aclara el mecanismo y no vuelve automáticamente a React/Angular.
- **OL2:** Preguntar por un concepto frontend pertinente sin módulo dedicado (por ejemplo, una API del navegador o un detalle de accesibilidad): se enseña en contexto sin bloquear por el currículo.
- **OL3:** Solicitar un caso nuevo fuera de Portal Ágora: el tutor crea/adapta un escenario y distingue los supuestos de los hechos verificados.
- **OL4:** Pedir un detalle avanzado del navegador o rendering sin completar el currículo: el tutor cubre los prerrequisitos mínimos y no impone una ruta completa.
- **OL5:** Preguntar por una dependencia backend desde un problema de UI: explica el contrato o mecanismo mínimo y conserva el foco frontend, salvo ampliación explícita.

## Checks de apertura y foco

- **OL1:** Pedir un ejemplo con una tecnología no incluida en la lista familiar: el tutor puede usarla si aclara el mecanismo y no vuelve automáticamente a React/Angular.
- **OL2:** Preguntar por un concepto frontend pertinente sin módulo dedicado (por ejemplo, una API del navegador o un detalle de accesibilidad): se enseña en contexto sin bloquear por el currículo.
- **OL3:** Solicitar un caso nuevo fuera de Portal Ágora: el tutor crea/adapta un escenario y distingue los supuestos de los hechos verificados.
- **OL4:** Pedir un detalle avanzado del navegador o rendering sin completar el currículo: el tutor cubre los prerrequisitos mínimos y no impone una ruta completa.
- **OL5:** Preguntar por una dependencia backend desde un problema de UI: explica el contrato o mecanismo mínimo y conserva el foco frontend, salvo ampliación explícita.

## Caso centinela

Un portal pierde rendimiento móvil después de añadir un paquete grande; algunos filtros muestran resultados antiguos y un flujo de compra puede reintentarse tras un timeout. El tutor debe primero explicar los mecanismos y estados involucrados, distinguir hipótesis de evidencia y definir cómo validar causas. No debe saltar directamente a «usar X framework», instalar una librería de estado o dividir la aplicación en microfrontends.


## Checks de configuración de Fuentes (v1.5.2, manuales)

- **SRC-01:** Las fuentes cargadas se reconocen por nombre individual; no se espera que ChatGPT conozca la carpeta original. No se cargan tres guías distintas como `README.md`.
- **SRC-02:** `INTERACTION_ENGINE.md`, `DECISION_ENGINE.md` y `PRACTICE_ENGINE.md` están como Fuentes, no como Instrucciones activas concatenadas; el framework conserva v1.4.1.
- **SRC-03:** Sin `LAB_GUIDE.md`, `/learn` y `/lab` siguen funcionando; sin `CONCEPT_MAP.md`, no se inventa su contenido. Se evita usar `ACCEPTANCE_CHECKS.md` como examen del estudiante.
- **SRC-04:** `ARCHITECTURE_DECISIONS_GUIDE.md` describe ADRs técnicos, mientras que `DECISION_ENGINE.md` desarrolla criterio; en el setup se distinguen ambas funciones.

Estas pruebas están definidas pero **no se consideran ejecutadas ni aprobadas** hasta verificar el tutor en un Proyecto real.
