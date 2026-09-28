# Engineering notes

These notes describe the engineering approach behind my Angular and mapping work.
Explore the public demos to try the behavior, or contact me to discuss architecture,
implementation and support for your application.

## Angular library maintenance: ng-openlayers

**Project:** [ng-openlayers — product and support](https://furtak.dev/projects/ng-openlayers/) · [live examples](https://ng-openlayers.furtak.dev/)
**My role:** library development, maintenance and integration support. Commercial access
and implementation support are arranged directly through [contact](mailto:kamil@furtak.dev).

**Problem.** OpenLayers creates maps, listeners and other mutable objects outside Angular. A declarative wrapper needs clear ownership when components are updated, replaced or destroyed. A successful demo alone does not establish that consumers can install and use the released package.

**Decisions.**

- Every component owns the OpenLayers objects it creates and disposes them on destroy; consumer-supplied objects stay with the consumer. Constructor-only options replace the owned object; everything else updates in place.
- Components are `OnPush` and the demo runs zoneless. Map creation, pointer handling and rendering run outside Angular's zone; observed outputs re-enter it for applications that still use Zone.js.
- Reusable wrapper components provide sources, styles and attribution through ancestor injection, so application teams can build their own composed components on top of the library.
- The delivery pipeline runs regression suites, browser scenarios against the production demo, and an independent Angular application that installs the built library package.

**What to try.**

- [Interactive drawing](https://ng-openlayers.furtak.dev/examples/draw-polygon/)
- [Measurement tools](https://ng-openlayers.furtak.dev/examples/measure/)
- [All 27 examples](https://ng-openlayers.furtak.dev/)
- [Discuss an integration or architecture review](mailto:kamil@furtak.dev)

**Boundary.** The wrapper has a documented API surface; it does not make every OpenLayers option dynamically mutable. Provider fixtures in browser tests and live provider behavior are separate checks. Coverage measures executed code, not the absence of every leak.

## The portfolio site itself

[furtak.dev](https://furtak.dev/) is an Angular application prerendered to static HTML.
GitHub Actions builds and verifies the site, then deploys the production files to my
hosting environment. The source repository is private. Content lives in typed data files,
pages are standalone components and metadata is generated per route.

The site introduces my services and ng-openlayers. It provides a direct point of contact
for consulting, implementation and support.

## Contributions reviewed by other maintainers

- **[bolt.diy #1322](https://github.com/stackblitz-labs/bolt.diy/pull/1322), merged.** Replaced the model selector's static dropdown with search, filtered results, keyboard navigation and focus handling.
- **[Hindsight #3656](https://github.com/vectorize-io/hindsight/pull/3656), merged.** The batch path built a schema from one configuration flag and sent its strictness setting from another. I aligned both decisions with the retain-scoped flag and added tests for both directions of the mismatch.

[Back to my profile](README.md) · [Services](https://furtak.dev/) · [Contact](mailto:kamil@furtak.dev)
