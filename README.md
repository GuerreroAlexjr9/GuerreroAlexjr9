<!--
  Alex Guerrero — GitHub Profile
  Frontend / Mobile Architect · React · React Native · TypeScript
  Available for consulting · Santa Marta, CO (UTC−5)
-->

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/banner-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="./assets/banner-light.svg">
    <img alt="Alex Guerrero — Frontend/Mobile Architect" src="./assets/banner-dark.svg" />
  </picture>
</p>

<p align="center">
  <a href="mailto:guerreroalexjr@gmail.com">
    <img alt="Available for consulting" src="https://img.shields.io/badge/Available%20for-Consulting-22C55E?style=flat-square&labelColor=0B0F19" />
  </a>
  <img alt="Based in Santa Marta, CO" src="https://img.shields.io/badge/Based%20in-Santa%20Marta%2C%20CO-38BDF8?style=flat-square&labelColor=0B0F19" />
  <img alt="UTC−5" src="https://img.shields.io/badge/Timezone-UTC%E2%88%925-94A3B8?style=flat-square&labelColor=0B0F19" />
  <img alt="Open to remote" src="https://img.shields.io/badge/Open%20to-Remote-818CF8?style=flat-square&labelColor=0B0F19" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/alexjrguerrero">LinkedIn</a> ·
  <a href="mailto:guerreroalexjr@gmail.com">Email</a> ·
  <a href="https://github.com/GuerreroAlexjr9/react-architecture-playground">Flagship repo</a>
</p>

<p align="center">
  <img alt="Flagship CI" src="https://img.shields.io/github/actions/workflow/status/GuerreroAlexjr9/react-architecture-playground/ci.yml?branch=main&label=react-architecture-playground%20%C2%B7%20CI&style=flat-square&labelColor=0B0F19" />
  <img alt="License" src="https://img.shields.io/github/license/GuerreroAlexjr9/react-architecture-playground?style=flat-square&labelColor=0B0F19" />
</p>

---

## Sobre mí

Diseño y evoluciono aplicaciones **web y móviles enterprise** en **React**, **React Native** y **TypeScript**.
Mi trabajo se concentra en **arquitectura modular**, **migraciones incrementales** desde bases legacy y **design systems** que sostienen el ritmo de equipos grandes.

Vengo de entornos donde compatibilidad, performance y trazabilidad **no son negociables**, y donde el delivery no puede frenarse para refactorizar. Mi enfoque es ese intermedio: **modernizar sin romper**.

---

## Consultoría

> **Disponible para engagements remotos** — equipos producto, plataformas internas y modernización de stacks frontend/mobile.

| Engagement | Cuándo aplica |
|---|---|
| **Architecture audit** | Tu app crece más rápido que su estructura: bordes difusos, regresiones constantes, equipos que se pisan. |
| **Migration roadmap** | Necesitas pasar de legacy (CRA, AngularJS, Webpack viejo, RN clásico) a un stack moderno sin congelar features. |
| **Design system bootstrap** | Quieres consistencia visual y de comportamiento entre productos sin reinventar componentes en cada squad. |
| **Hands-on advisory** | Tu equipo necesita un arquitecto embebido part-time para guardrails, code review y decisiones técnicas. |

➜ **[guerreroalexjr@gmail.com](mailto:guerreroalexjr@gmail.com?subject=Consulting%20inquiry)** · respuesta en 48h.

---

## Cómo aporto valor

- **Arquitectura por dominios** — feature-based boundaries, project references de TypeScript y reglas de ESLint que evitan acoplamientos antes del PR.
- **Migraciones controladas** — strangler pattern, feature flags y métricas para reemplazar legacy sin congelar el roadmap del producto.
- **Design systems componibles** — tokens, primitives y componentes accesibles (WAI-ARIA) listos para web y móvil, con governance clara.
- **Testing como contrato** — pirámide pragmática (unit + integration + e2e crítico) y CI con budgets que bloquean regresiones, no que decoran.
- **Performance medible** — Core Web Vitals y startup móvil con presupuestos versionados, no “sentir que va más rápido”.

---

## Stack

| Capa | Tecnologías |
|---|---|
| **Core** | React · React Native · TypeScript · Next.js |
| **Arquitectura** | Feature-based modules · Monorepo (pnpm/turbo) · Design Systems |
| **Calidad** | Vitest · Jest · Testing Library · Playwright · ESLint · TS project refs |
| **Estado & Datos** | Zustand · Redux Toolkit · React Query · GraphQL · REST |
| **Plataforma** | GitHub Actions · AWS · Firebase · Vercel |

<p>
  <img alt="React" src="https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB&style=flat-square" />
  <img alt="React Native" src="https://img.shields.io/badge/React%20Native-20232A?logo=react&logoColor=61DAFB&style=flat-square" />
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white&style=flat-square" />
  <img alt="Next.js" src="https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white&style=flat-square" />
</p>

---

## Proyectos insignia

### [`react-architecture-playground`](https://github.com/GuerreroAlexjr9/react-architecture-playground)
Referencia ejecutable de arquitectura escalable en React: feature-based modules, route guards, capa de estado, testing y CI listos para producción.
**Docs:** [`/docs/spec.md`](https://github.com/GuerreroAlexjr9/react-architecture-playground/blob/main/docs/spec.md) · [`/docs/architecture.md`](https://github.com/GuerreroAlexjr9/react-architecture-playground/blob/main/docs/architecture.md) · [`/docs/decisions.md`](https://github.com/GuerreroAlexjr9/react-architecture-playground/blob/main/docs/decisions.md)

### Próximos
- **`react-native-architecture-playground`** — equivalente móvil con navegación, módulos nativos y CI multi-plataforma.
- **`design-system-starter`** — base mínima viable para un DS multi-producto (tokens, primitives, governance).

---

## Mindset de arquitectura

```mermaid
flowchart LR
  subgraph Apps["Apps"]
    Web["Web · Next.js"]
    Mobile["Mobile · React Native"]
  end

  subgraph Domain["Domain Layer · feature-based"]
    F1["Feature A"]
    F2["Feature B"]
    F3["Feature C"]
  end

  subgraph Cross["Cross-cutting"]
    DS["Design System"]
    State["State"]
    Services["Services / API"]
    Tests["Testing & CI"]
  end

  Web --> Domain
  Mobile --> Domain
  Domain --> DS
  Domain --> State
  Domain --> Services
  Services --> API[("Backend / BFF")]
  Domain --> Tests
  DS --> Tests
  Services --> Tests

  classDef boundary fill:#0B0F19,stroke:#38BDF8,stroke-width:1.5px,color:#F8FAFC;
  classDef cross fill:#111827,stroke:#818CF8,stroke-width:1px,color:#CBD5E1;
  class Domain,F1,F2,F3 boundary;
  class DS,State,Services,Tests cross;
```

**Principios que aplico:**
1. Las **features no se conocen entre sí**; comparten contratos, no implementaciones.
2. El **design system** es la única fuente de UI; nada de variantes ad-hoc por squad.
3. Los **servicios** son una capa fina sobre la red; la lógica de negocio vive en el dominio.
4. **Testing** acompaña la arquitectura, no la persigue.
5. Toda decisión relevante queda en un **ADR** versionado.

---

## Métricas

<p align="center">
  <img alt="GitHub metrics" src="./.github/metrics/github-metrics.svg" />
</p>

<p align="center">
  <img alt="Languages" src="./.github/metrics/github-metrics-langs.svg" width="49%" />
  <img alt="Activity calendar" src="./.github/metrics/github-metrics-calendar.svg" width="49%" />
</p>

<sub>Generado automáticamente con <a href="https://github.com/lowlighter/metrics">lowlighter/metrics</a> · refresco diario.</sub>

---

<details>
<summary><strong>🇬🇧 Read in English</strong></summary>

### About

I design and evolve **enterprise web and mobile apps** in **React**, **React Native** and **TypeScript**. My focus is **modular architecture**, **incremental migrations** out of legacy stacks, and **design systems** that scale across multiple teams.

I work in environments where compatibility, performance and traceability are non-negotiable, and where delivery can’t freeze for a rewrite. My job sits exactly there: **modernize without breaking**.

### Consulting

Available for **remote engagements** — product teams, internal platforms and frontend/mobile modernization.

| Engagement | When it fits |
|---|---|
| **Architecture audit** | The codebase outgrew its structure: blurry boundaries, recurring regressions, teams stepping on each other. |
| **Migration roadmap** | You need to move off legacy (CRA, AngularJS, old Webpack, classic RN) without freezing features. |
| **Design system bootstrap** | You want visual and behavioral consistency across products without re-inventing components per squad. |
| **Hands-on advisory** | Your team needs a part-time embedded architect for guardrails, reviews and technical decisions. |

➜ **[guerreroalexjr@gmail.com](mailto:guerreroalexjr@gmail.com?subject=Consulting%20inquiry)** · reply within 48h.

### How I add value

- **Domain-driven frontend** — feature-based boundaries, TS project references and ESLint rules that prevent coupling before the PR.
- **Controlled migrations** — strangler pattern, feature flags and metrics to replace legacy without freezing the roadmap.
- **Composable design systems** — tokens, primitives and accessible components (WAI-ARIA) for web and mobile, with clear governance.
- **Testing as a contract** — pragmatic pyramid (unit + integration + critical e2e) and CI budgets that block regressions instead of decorating.
- **Measurable performance** — Core Web Vitals and mobile startup with versioned budgets, not “feels faster”.

</details>

---

<p align="center">
  <strong>¿Necesitas modernizar un frontend, migrar una app legacy o escalar un design system?</strong><br/>
  <sub>Need to modernize a frontend, migrate a legacy app or scale a design system?</sub>
</p>

<p align="center">
  <a href="mailto:guerreroalexjr@gmail.com?subject=Consulting%20inquiry">
    <img alt="Email" src="https://img.shields.io/badge/Let%27s%20talk-guerreroalexjr%40gmail.com-22C55E?style=for-the-badge&labelColor=0B0F19" />
  </a>
  <a href="https://www.linkedin.com/in/alexjrguerrero">
    <img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-alexjrguerrero-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0B0F19" />
  </a>
</p>
<!--
Perfil: Alex Guerrero (GuerreroAlexjr9)
Objetivo: posicionamiento como Arquitecto Frontend/Mobile + consultoría
-->

<p align="center">
  <img src="./assets/hero.png" alt="Alex Guerrero — Frontend/Mobile Architect" />
</p>

<h1 align="center">Alex Guerrero</h1>

<p align="center">
  <strong>Arquitecto Frontend/Mobile</strong> · React / React Native · TypeScript · Arquitectura modular · Migraciones enterprise
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/TU_HANDLE/">LinkedIn</a> ·
  <a href="mailto:TU_EMAIL@DOMINIO.com">Email</a> ·
  <a href="https://github.com/GuerreroAlexjr9/react-architecture-playground">Proyecto insignia</a>
</p>

<p align="center">
  <img alt="CI" src="https://img.shields.io/github/actions/workflow/status/GuerreroAlexjr9/react-architecture-playground/ci.yml?branch=main" />
  <img alt="License" src="https://img.shields.io/github/license/GuerreroAlexjr9/react-architecture-playground" />
</p>

## Sobre mí

Soy **Arquitecto Frontend/Mobile** con foco en construir y evolucionar aplicaciones **enterprise** en **React** y **React Native** (TypeScript-first).

Trabajo con arquitecturas modulares y participo en iniciativas de **modernización y migración** en entornos de alta exigencia, priorizando compatibilidad, performance, trazabilidad y calidad sin frenar el delivery.

### En qué te puedo ayudar

- **Arquitectura Frontend/Mobile**: estructura por dominios (feature-based), boundaries, convenciones y guardrails.
- **Migraciones sin trauma**: legacy → arquitecturas modernas, estrategias incrementales y control de riesgo.
- **Design Systems**: componentes reutilizables, accesibilidad y consistencia para equipos grandes.
- **Testing & Quality**: unit/integration testing, CI y reducción de regresiones.
- **Performance**: optimización de carga y navegación, medición y budgets.

## Stack principal

**Core**
- React · React Native · TypeScript · Next.js
- Arquitectura modular · Design Systems · Testing (Vitest/Jest)

**Plataforma**
- GraphQL/REST · AWS/Firebase · CI/CD (GitHub Actions)

<p>
  <img alt="React" src="https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB" />
  <img alt="React Native" src="https://img.shields.io/badge/React%20Native-20232A?logo=react&logoColor=61DAFB" />
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white" />
  <img alt="Next.js" src="https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white" />
  <img alt="Vitest" src="https://img.shields.io/badge/Vitest-6E9F18?logo=vitest&logoColor=white" />
  <img alt="Jest" src="https://img.shields.io/badge/Jest-C21325?logo=jest&logoColor=white" />
</p>

## Proyectos destacados

- **react-architecture-playground** → arquitectura escalable (feature-based), route guards, store, testing, CI y docs.
  - Repo: https://github.com/GuerreroAlexjr9/react-architecture-playground
  - Docs: `/docs/spec.md` · `/docs/architecture.md` · `/docs/decisions.md`

> Siguiente (en construcción):
> - react-native-architecture-playground
> - design-system-starter

## Arquitectura de referencia

```mermaid
flowchart LR
  UI[UI: Web / Mobile] --> Router[Routing & Navigation]
  Router --> Features[Features (dominios)]
  Features --> Shared[Shared (UI Kit / utils)]
  Features --> State[State (Zustand/Redux)]
  Features --> Services[Services (API Layer)]
  Services --> API[(Backend / BFF)]
  State --> Tests[Tests (unit/integration)]
  Services --> Tests
  Shared --> Tests