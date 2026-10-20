# CASEBOOK — Frontend Architecture & Design v1.5.1

Los casos de este archivo son ejemplos iniciales, no un conjunto cerrado. Portal Ágora es un caso conductor opcional para construir continuidad, no una parada obligatoria de cada sesión. Selecciona o crea casos nuevos si explican mejor el concepto o prueban transferencia; etiqueta supuestos ficticios y distingue los hechos reales que requieran verificación. El currículo y este casebook pueden evolucionar, pero no añadas módulos por cada curiosidad ni cambies IDs sin una revisión deliberada.

## Caso conductor: Portal Ágora (escenario ficticio)

Portal Ágora es una plataforma web con páginas públicas indexables, una zona autenticada y un flujo de compra. Los datos y restricciones que aparecen a continuación son **supuestos didácticos**, no resultados reales. No existe una solución predeterminada; cada decisión debe explicar qué evidencia faltaría para confirmar que conviene.

### Caso base

- Dos equipos mantienen distintas áreas del producto.
- Las páginas públicas necesitan indexación y tiempos de carga razonables en móviles.
- La zona autenticada presenta filtros y listas que dependen de datos remotos.
- El checkout puede experimentar timeouts y reintentos.
- El equipo quiere evitar que cada mejora introduzca una complejidad operativa que no puede sostener.

### Iteraciones

| Iteración | Situación | Conceptos que conviene entender antes de decidir | Evidencia posible |
|---|---|---|---|
| F-0 | Se diseña el MVP con páginas públicas y checkout interactivo. | Rendering, SEO, interactividad, latencia, caché y coste de operación. | Decisión razonada entre MPA/SPA/SSR/SSG o enfoque híbrido, con supuestos. |
| F-1 | Los filtros pierden estado al navegar y a veces muestran datos antiguos. | UI state vs server state, caché, invalidación, URL state, carreras y estados de error. | Tabla de estados/transiciones y explicación de una secuencia que produce datos obsoletos. |
| F-2 | Tras añadir una librería de gráficos, la experiencia móvil parece más lenta. | Descarga/parse/execute, main thread, rendering, code splitting, medición y confusores. | Hipótesis priorizadas y plan de medición; si se mide, entorno y resultados reales. |
| F-3 | El producto crece a cuatro equipos con distintas cadencias de entrega. | Límites modulares, ownership, acoplamiento, runtime compartido, coordinación y coste de MFE. | Comparación entre monolito modular, monorepo, paquetes compartidos y microfrontends. |
| F-4 | Tras un timeout, el usuario vuelve a pulsar comprar y la UI muestra un estado ambiguo. | Estado de operación, incertidumbre de red, idempotencia contractual, reintentos y reconciliación. | Diagrama de estados de UI y contrato de interacción que no inventa un éxito definitivo. |
| F-5 | Una revisión detecta un flujo susceptible a XSS y componentes difíciles de usar solo con teclado. | Fronteras de confianza, escape/sanitización contextual, CSP, semántica, foco y pruebas. | Threat model y plan de validación de accesibilidad, con límites de cada mitigación. |
| F-6 | Una versión nueva de un módulo compartido rompe una vista de otra área. | Contratos, versionado, compatibilidad, pruebas de integración, observabilidad y rollback. | Plan de compatibilidad/rollback y señales para detectar impacto real. |
| F-7 | Un dashboard con tablas grandes se vuelve lento con datos de alto volumen. | Coste de DOM, virtualización, paginación, memoria, accesibilidad y carga cognitiva. | Comparación condicionada por interacción, tamaño de datos y necesidades de navegación. |

## Guía de razonamiento

Antes de proponer una solución:
1. Aclarar qué observa el usuario y qué objetivo se incumple.
2. Separar hechos proporcionados, supuestos didácticos e hipótesis.
3. Explicar el mecanismo causal relevante: qué estado cambia, qué evento lo dispara y qué límite aparece.
4. Definir qué señal, experimento o prueba podría distinguir las hipótesis.
5. Comparar al menos una alternativa viable y su coste cuando la decisión lo amerite.
6. Verificar si la conclusión sigue siendo válida al cambiar una restricción importante.

No es obligatorio usar todos los pasos en cada respuesta ni producir un ADR/código por defecto. El caso no es un examen permanente y no requiere experiencia previa de otro Proyecto SETS.

## Transferencias

Usar, cuando ayude, un dashboard SaaS B2B con tablas grandes, un portal público indexable, una aplicación offline-first, una plataforma educativa accesible o un shell de producto con múltiples equipos. Explicar qué principios permanecen y qué restricciones cambian.
