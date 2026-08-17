# MAKSIM BUREEV

**Senior Frontend Engineer · Vue 3 · TypeScript · Frontend Architecture, Reliability & DX**

Almaty, Kazakhstan · +7 705 905 39-62 · maxxborer@gmail.com  
LinkedIn: linkedin.com/in/maxxborer · GitHub: github.com/maxxborer · Organization: github.com/maseaaao

Open to remote work and relocation · Russian — Native · English — B1

## PROFILE

Hands-on Senior Frontend Engineer with 7+ years across e-commerce, fintech and govtech. I own frontend technical decisions across several projects—from architecture and complex migrations to reliability, performance and production rollout—and build shared standards, developer tooling and engineering metrics used by multiple teams.

## CORE SKILLS

**Frontend:** Vue 3, Nuxt 3/4, TypeScript, JavaScript, Composition API, Pinia, Vuex, HTML5, CSS/SCSS. **Architecture & Data:** GraphQL, REST API, HTTP, Axios, Apollo Client, Node.js, feature flags. **Quality & Delivery:** Vite, Vitest, Playwright, Git, GitLab CI/CD, Sentry, observability, performance.

## EXPERIENCE

### Kaspi.kz · Almaty, Kazakhstan
**Senior Frontend Engineer · Technical Lead** · Jan 2024 — Present

- **Eliminated parallel maintenance of critical order flows across two Vue SPAs.** Replaced an undocumented SAP Hybris integration with documented GraphQL and service APIs. Owned architecture and delivery end to end—contract analysis, adapters, regression, monitoring and a staged **10% → 100% rollout**—then retired the legacy path and **7,200+ LOC**.
- **Standardized frontend engineering across 13 product repositories.** Built and own a shared Vue/TypeScript package centralizing TypeScript, linting, browser-support, build and CI defaults. Automated recurring reviewer and PR-Agent feedback, reducing comments from roughly **25 to 10 per MR**, and centralized Renovate-driven configuration updates.
- **Halved initial-load time and preserved in-progress actions when access tokens expired.** Removed redirect-based authentication in favor of stateless REST, then built a shared refresh/retry queue for Axios and Apollo: requests receiving 401 stay pending while the token refreshes in the background and replay after success. Cold start fell from roughly **10 to 5 seconds**; warm start from **5 to 1–2 seconds**.
- **Built non-blocking observability from HTML bootstrap through Vue runtime and cut frontend error volume from 10–15k to approximately 4k events per day.** A minimal Sentry core loads with HTML to capture pre-Vue failures; Vue integrations, tracing, replay, source maps and diagnostic context—feature flags, A/B tests, viewport and authentication state—attach lazily. Early errors are preserved without delaying application startup.
- **Cut Speed Index by 52% despite the application's primary pods being limited to HTTP/1.1.** Designed a separate HTTP/2 CDN delivery pod and a two-minute version gate: asset traffic moves to CDN only after origin and CDN versions match and stays on origin on mismatch. Like-for-like Lighthouse runs improved Speed Index from **16.9 to 8.1 seconds**; TBT fell by **40%** and LCP by **17%**.

### Samgau Holding · Astana, Kazakhstan
**Senior Frontend Developer** · Oct 2022 — Jan 2024

- Migrated a React application from Webpack to Vite: production build time fell from **36 to 6 minutes** and local dev-server startup from **1.5 minutes to 1–5 seconds**. Removed legacy packages and embedded quality checks in CI.
- Built a JSON-driven tax-form platform: schemas define fields and behavior while the frontend handles rendering and validation, reducing duplication when adding sections.

### Digital Economy League · Remote
**Middle Frontend Developer** · Nov 2021 — Oct 2022

- Introduced CI/CD with isolated QA environments per developer and domain-oriented organization in a banking SPA with **400+ components**.

### OCRV · Remote
**Middle Frontend Developer** · Aug 2020 — Nov 2021

- Built an employee-feedback platform serving **85,000 employees** across **10,000 organizational units**, with virtualized lists and drill-down analytics. Added a Node.js/Express BFF that consolidated **10+ backend requests into a single frontend response**, reducing browser-side orchestration and simplifying an inefficient API.

### BuzzGuru (Wisebits Group) · Limassol, Cyprus
**Junior Frontend Developer** · Mar 2019 — Aug 2020

- Developed **10+** SVG/Canvas analytics chart types and contributed to a move from Bootstrap and third-party UI kits to a proprietary component library.

## INTERNAL ENGINEERING PRODUCTS

### Review Pulse Check · TypeScript, GitLab API, CI/CD

Built and deployed a code-review health platform across **15+ repositories and 5+ teams**. Scheduled CI/CD publishes auditable reports every three days on review coverage, missed reviews, median and P90 first response, workload and trends—helping teams identify process bottlenecks without scoring individuals.

### MR Message Generator · Nuxt 4, Vue 3, TypeScript, GitLab API

Built an internal product that generates standardized review and release messages from GitLab MR and tag URLs, with configurable templates, validation and history for different workflows. An internal survey found that **one-third of engineers use it daily**.

## EDUCATION

**Togliatti State University** · BSc, Mathematical Software and Information Systems Administration · 2020
