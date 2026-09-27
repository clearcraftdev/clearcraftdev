<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/profile-banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/profile-banner-light.svg">
  <img alt="Kamil Furtak — Senior Angular Engineer. Angular, TypeScript and geospatial UI." src="assets/profile-banner-light.svg" width="1440">
</picture>

**Senior Angular Engineer · 13 years in enterprise web development · GIS & interactive maps · UI modernization · Reusable libraries**

I build Angular frontends for complex, domain-heavy products: GIS and map-based applications, document management and public-sector systems. My focus is preserving user workflows during UI changes, designing reusable component APIs, and making state, lifecycle and integration behavior testable. I also maintain [ng-openlayers](https://github.com/kamilfurtak/ng-openlayers), an Angular library for OpenLayers maps with 17 releases across Angular 17–22.

| At a glance | |
| --- | --- |
| **Role** | Senior Angular Engineer / frontend architecture |
| **Experience** | 13 years in enterprise web applications · 9+ years with Angular |
| **Domains** | GIS & web mapping, geodesy and cartography, document management, public sector |
| **Core stack** | Angular, TypeScript, RxJS, Nx, OpenLayers |
| **Open source** | Maintainer of [ng-openlayers](https://www.npmjs.com/package/ng-openlayers) · merged changes in [bolt.diy](https://github.com/stackblitz-labs/bolt.diy/pull/1322) and [Hindsight](https://github.com/vectorize-io/hindsight/pull/3656) |
| **Open to** | Senior Angular and frontend-architecture roles |
| **Contact** | [kamil@furtak.dev](mailto:kamil@furtak.dev) · [LinkedIn](https://linkedin.com/in/kamilfurtak) |

[Portfolio & demos](https://furtak.dev/) · [Experience & skills](https://furtak.dev/hire-me/#experience) · [Engineering decisions & review guide](engineering-notes.md) · [Work with me](https://furtak.dev/hire-me/)

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
| **GIS & web mapping** | OpenLayers; OSM, XYZ, WMS, WMTS, ArcGIS and GeoJSON sources; map projections and coordinate transformation (Proj4); drawing, editing, snapping, selection and measurement |
| **Architecture & delivery** | Nx monorepos and generators, incremental UI modernization, CI/CD, Git, Docker, Linux, AI-assisted workflows (MCP) |
| **Testing & quality** | Jasmine, Karma, Cypress, Playwright, axe accessibility checks, package-consumer validation, code review |
| **Backend & integration** | REST, OpenAPI, Java/Spring, C#/.NET, NestJS/Node.js, PHP/Symfony, SAML, SOAP/WSDL, SQL |

## Selected engineering work

### [ng-openlayers](https://github.com/kamilfurtak/ng-openlayers) [![npm version](https://img.shields.io/npm/v/ng-openlayers.svg)](https://www.npmjs.com/package/ng-openlayers)

**Role: maintainer.** A published Angular library with 27 interactive map examples and 17 releases across Angular 17–22. My work includes component and event lifecycle ownership, projection changes, API compatibility and release validation.

The engineering challenge is connecting imperative OpenLayers objects to Angular's component lifecycle. The repository includes regression tests and an independent consumer that installs the built npm package.

[Try drawing on a map](https://ng-openlayers.furtak.dev/examples/draw-polygon/) · [Source & validation](https://github.com/kamilfurtak/ng-openlayers/blob/master/docs/validation.md) · [npm package](https://www.npmjs.com/package/ng-openlayers)

### [Angular UI modernization](https://furtak.dev/angular-ui-modernization-case-study/)

**Focus: replacing a table renderer while preserving feature behavior.** This Angular workbench keeps its state and form outside the table renderer. Switching between native and PrimeNG tables retains filtering, sorting, selection and draft edits.

Try selecting a case, changing the filter and writing a draft, then switch tables. The source also covers failed requests, retry and unavailable browser storage. Independent sample with fictional data.

[Try the workbench](https://furtak.dev/angular-ui-modernization-case-study/) · [Code & tests](https://github.com/kamilfurtak/kamilfurtak.github.io/tree/main/reference-sources/angular-ui-modernization-case-study/demo) · [Decisions & scope](engineering-notes.md#ui-modernization)

### [Identity integration architecture](https://furtak.dev/epuap-login-gov-integration-portfolio/)

A written case study of browser/API responsibility, generated contracts and failure boundaries around SAML and SOAP/WSDL. It shows how I reason about integration tradeoffs from the frontend side.

[Read the architecture](https://furtak.dev/epuap-login-gov-integration-portfolio/docs/architecture.html)

## Accepted open-source contributions

Selected changes accepted by other open-source projects:

- **[bolt.diy #1322](https://github.com/stackblitz-labs/bolt.diy/pull/1322)** — added model search and keyboard navigation to the model selector, including focus handling and filtering.
- **[Hindsight #3656](https://github.com/vectorize-io/hindsight/pull/3656)** — fixed disagreement between schema generation and the batch retain configuration; added regression tests for both conflicting settings.

## How I work

I keep feature state separate from rendering, define resource ownership, and test failure paths alongside successful flows. I document the limits of each example so reviewers can distinguish demonstrated behavior from a design proposal.

I use AI tools to support implementation; design decisions, source review and verification remain my responsibility.

Building a product with a complex Angular frontend or interactive maps? [Email me](mailto:kamil@furtak.dev) or [connect on LinkedIn](https://linkedin.com/in/kamilfurtak).
