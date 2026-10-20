# REFERENCES — Frontend Architecture & Design

Seguir la política de referencias de `sets-framework/docs/REFERENCE_POLICY.md`. Consultar la documentación correspondiente a la versión del navegador, framework, herramientas y entorno de render; una página de documentación no demuestra que un comportamiento se haya medido en el proyecto.

## Plataforma web y navegador

- **MDN Web Docs:** https://developer.mozilla.org/en-US/docs/Web — HTML, CSS, JavaScript, HTTP, DOM, APIs, seguridad y compatibilidad.
- **WHATWG HTML Living Standard:** https://html.spec.whatwg.org/ — semántica y comportamiento de HTML.
- **W3C CSS:** https://www.w3.org/Style/CSS/ — estándares y especificaciones CSS.

## Rendimiento y rendering

- **web.dev — Performance:** https://web.dev/performance/ — Core Web Vitals, estrategias de medición y optimización.
- **Chrome for Developers — Performance:** https://developer.chrome.com/docs/devtools/performance/ — análisis de performance en DevTools; resultados dependen del entorno.
- **Chrome UX Report:** https://developer.chrome.com/docs/crux/ — datos de experiencia de usuarios reales con límites de cobertura y segmentación.

## Accesibilidad

- **W3C WAI:** https://www.w3.org/WAI/ — recursos y estándares de accesibilidad web.
- **WCAG 2.2:** https://www.w3.org/TR/WCAG22/ — criterios de conformidad; combinar herramientas automáticas con evaluación manual y con usuarios.

## Seguridad

- **OWASP Cheat Sheet Series:** https://cheatsheetseries.owasp.org/ — XSS, CSRF, CSP, gestión de sesiones y controles por contexto.
- **OWASP Web Security Testing Guide:** https://owasp.org/www-project-web-security-testing-guide/ — enfoque de pruebas de seguridad web.

## Frameworks y arquitectura modular

- **React Documentation:** https://react.dev/ — modelo de componentes, rendering, estado y APIs de React.
- **Angular Documentation:** https://angular.dev/ — componentes, reactividad, rendering, DI y APIs de Angular.
- **Vue Documentation:** https://vuejs.org/guide/introduction.html — modelo de componentes y reactividad de Vue.
- **Martin Fowler — Micro Frontends:** https://martinfowler.com/articles/micro-frontends.html — beneficios, riesgos y límites de la arquitectura MFE; no es una recomendación universal.
- **Module Federation:** https://module-federation.io/ — consultar compatibilidad, runtime y versión antes de aplicar.

## Testing

- **Testing Library:** https://testing-library.com/docs/ — pruebas desde la perspectiva de uso de la interfaz.
- **Playwright:** https://playwright.dev/docs/intro — automatización end-to-end y su alcance.
- **axe-core:** https://github.com/dequelabs/axe-core — comprobaciones automáticas de accesibilidad; no cubre toda la evaluación manual.

## Criterio de uso

Primero definir la pregunta técnica y el contexto. Preferir estándares y documentación oficial para comportamiento normativo; usar artículos como contexto y contrastarlos con documentación vigente. Distinguir recomendación, especificación, inferencia y resultado medido.
