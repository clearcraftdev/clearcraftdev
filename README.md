<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/profile-banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/profile-banner-light.svg">
  <img alt="Kamil Furtak — Senior Angular Engineer. Angular, TypeScript and geospatial UI." src="assets/profile-banner-light.svg" width="1440">
</picture>

**Senior Angular Engineer · 13 years in enterprise web development · advanced interfaces & GIS · maintainer of ng-openlayers**

I design and build advanced Angular interfaces — data-heavy workbenches, editors and map-based tools — and the reusable libraries behind them. Most of that work happens in domain-heavy products: GIS and cartography, document management and public-sector systems. In the open, I maintain [ng-openlayers](https://github.com/kamilfurtak/ng-openlayers), an Angular library for OpenLayers with 17 releases across Angular 17–22.

| At a glance | |
| --- | --- |
| **Role** | Senior Angular Engineer / frontend architecture |
| **Experience** | 13 years in enterprise web applications · 9+ years with Angular |
| **Domains** | Advanced UIs for domain experts, GIS & web mapping, document management, public sector |
| **Core stack** | Angular, TypeScript, RxJS & Signals, Nx, OpenLayers |
| **Open source** | Maintainer of [ng-openlayers](https://www.npmjs.com/package/ng-openlayers) · merged changes in [bolt.diy](https://github.com/stackblitz-labs/bolt.diy/pull/1322) and [Hindsight](https://github.com/vectorize-io/hindsight/pull/3656) |
| **Open to** | Senior Angular and frontend-architecture roles |
| **Contact** | [kamil@furtak.dev](mailto:kamil@furtak.dev) · [LinkedIn](https://linkedin.com/in/kamilfurtak) |

[Portfolio](https://furtak.dev/) · [ng-openlayers overview](https://furtak.dev/projects/ng-openlayers/) · [Experience & skills](https://furtak.dev/hire-me/#experience) · [Engineering notes](engineering-notes.md)

## ng-openlayers — the flagship [![npm version](https://img.shields.io/npm/v/ng-openlayers.svg)](https://www.npmjs.com/package/ng-openlayers) [![CI](https://github.com/kamilfurtak/ng-openlayers/actions/workflows/ci.yml/badge.svg)](https://github.com/kamilfurtak/ng-openlayers/actions/workflows/ci.yml)

**Maps, the Angular way.** Declarative OpenLayers components for Angular: map, view, layers, sources, styles, controls and interactions composed in templates, with typed inputs and events and full access to the underlying instances.

| | |
| --- | --- |
| **27** | interactive examples, each linked to its TypeScript source |
| **17** | releases across Angular 17–22, one major at a time |
| **230+** | unit tests and 48 browser scenarios per release |
| **94%** | line coverage in the library, enforced in CI |

What the library demonstrates beyond maps:

- **Public API design** — a declarative surface over an imperative engine: typed inputs, event outputs, composition through templates and ancestor injection.
- **Lifecycle ownership** — each component owns the OpenLayers objects it creates and disposes them; consumer-supplied objects stay with the consumer.
- **Performance by default** — OnPush components, zoneless change detection, pointer and render work outside Angular's zone.
- **Release engineering** — the built npm tarball is installed into an independent Angular app in CI; browser suites run against the production example site.

[Try the 27 live examples](https://ng-openlayers.furtak.dev/) · [Source & tests](https://github.com/kamilfurtak/ng-openlayers) · [Validation scope](https://github.com/kamilfurtak/ng-openlayers/blob/master/docs/validation.md) · [Project overview](https://furtak.dev/projects/ng-openlayers/)

## Experience

**13 years** of building enterprise web applications, **9+ years** with Angular — from jQuery and Knockout to Nx monorepos and signals.

#### 2022 – present · Senior Angular Engineer / Frontend Architecture

Angular frontend architecture for GIS, geodesy and cartography, document-management and public-sector systems.

- Nx monorepos, shared Angular libraries and reusable UI components for domain-heavy workflows.
- Migration of legacy Kendo/jQuery portals to Angular, with new interfaces working alongside established workflows.
- OpenLayers map features: spatial object interaction, sketching and editing.
- Nx generators and development automation; code review, integration debugging and automated tests.

#### 2020 – 2022 · Senior Angular Frontend Developer

Angular SPAs with modular routing, shared components and typed REST integrations. Improved structure and performance with lazy loading, AOT builds and change-detection strategies. Kendo UI and Angular Material forms with Jasmine, Karma and Cypress regression testing.

#### 2017 – 2019 · Angular Frontend Developer

Reusable components, services, routing and route guards for business and geospatial workflows. Code reviews, CI/CD and automated testing for maintainable, reliable releases.

#### 2013 – 2016 · Full-stack JavaScript Developer

JavaScript, jQuery, Knockout and Kendo UI on PHP/Symfony and Java backends with REST APIs and Oracle SQL.

**Education & languages:** MSc, AGH University of Science and Technology · postgraduate diploma in Java web development · Polish (native), English (B2, working proficiency).

## Skills

| Area | Skills |
| --- | --- |
| **Angular & TypeScript** | Angular (signals, RxJS), reusable component APIs and libraries, lazy loading, change-detection strategies, Kendo UI, PrimeNG, Angular Material, Formly |
| **Advanced interfaces** | Data-heavy workbenches, editors, dialogs and multi-step forms; state ownership, keyboard and accessibility behavior, workflows that survive UI changes |
| **GIS & web mapping** | OpenLayers; OSM, XYZ, WMS, WMTS, ArcGIS and GeoJSON sources; map projections and coordinate transformation (Proj4); drawing, editing, snapping, selection and measurement |
| **Architecture & delivery** | Nx monorepos and generators, incremental UI modernization, CI/CD, Git, Docker, Linux, AI-assisted workflows (MCP) |
| **Testing & quality** | Jasmine, Karma, Cypress, Playwright, axe accessibility checks, package-consumer validation, code review |
| **Backend & integration** | REST, OpenAPI, Java/Spring, C#/.NET, NestJS/Node.js, PHP/Symfony, SAML, SOAP/WSDL, SQL |

## Accepted open-source contributions

- **[bolt.diy #1322](https://github.com/stackblitz-labs/bolt.diy/pull/1322)** — added model search and keyboard navigation to the model selector, including focus handling and filtering.
- **[Hindsight #3656](https://github.com/vectorize-io/hindsight/pull/3656)** — fixed disagreement between schema generation and the batch retain configuration; added regression tests for both conflicting settings.

## How I work

I keep feature state separate from rendering, define resource ownership, and test failure paths alongside successful flows. I document the limits of each example so reviewers can distinguish demonstrated behavior from a design proposal. AI tools support my implementation work; design decisions, source review and verification remain mine.

Building a product with a complex Angular frontend or interactive maps? [Email me](mailto:kamil@furtak.dev) or [connect on LinkedIn](https://linkedin.com/in/kamilfurtak).
