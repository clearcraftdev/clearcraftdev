# Engineering notes

These notes connect my public work to the engineering decisions behind it.
Start with the live examples for behavior, then follow the source and tests for detail.

## Angular library maintenance: ng-openlayers

**Project:** [ng-openlayers](https://github.com/kamilfurtak/ng-openlayers) · [live examples](https://ng-openlayers.furtak.dev/) · [overview on furtak.dev](https://furtak.dev/projects/ng-openlayers/)
**My role:** maintainer of a library that builds on the existing Angular/OpenLayers wrapper work credited in its README.

**Problem.** OpenLayers creates maps, listeners and other mutable objects outside Angular. A declarative wrapper needs clear ownership when components are updated, replaced or destroyed. A successful demo alone does not establish that consumers can install and use the released package.

**Decisions.**

- Every component owns the OpenLayers objects it creates and disposes them on destroy; consumer-supplied objects stay with the consumer. Constructor-only options replace the owned object; everything else updates in place.
- Components are `OnPush` and the demo runs zoneless. Map creation, pointer handling and rendering run outside Angular's zone; observed outputs re-enter it for applications that still use Zone.js.
- Reusable wrapper components provide sources, styles and attribution through ancestor injection, so application teams can build their own composed components on top of the library.
- Releases track Angular majors one at a time (17 → 22, 17 releases). Each release runs the regression suites, the browser scenarios against the production example site, and an independent Angular application that installs the built npm tarball.

**What to inspect.**

- [Interactive drawing example](https://ng-openlayers.furtak.dev/examples/draw-polygon/)
- [Map lifecycle tests](https://github.com/kamilfurtak/ng-openlayers/blob/master/libs/ng-openlayers/src/lib/map-lifecycle.spec.ts)
- [Projection state tests](https://github.com/kamilfurtak/ng-openlayers/blob/master/libs/ng-openlayers/src/lib/view-projection-state.spec.ts)
- [Independent package consumer](https://github.com/kamilfurtak/ng-openlayers/tree/master/compatibility/angular22)
- [Validation scope and limitations](https://github.com/kamilfurtak/ng-openlayers/blob/master/docs/validation.md)
- [Angular 22 migration guide](https://github.com/kamilfurtak/ng-openlayers/blob/master/docs/angular-22-migration.md)

**Boundary.** The wrapper has a documented API surface; it does not make every OpenLayers option dynamically mutable. Provider fixtures in browser tests and live provider behavior are separate checks. Coverage measures executed code, not the absence of every leak.

## The portfolio site itself

[furtak.dev](https://furtak.dev/) is an Angular 22 application prerendered to static HTML, with its
[source in the same repository](https://github.com/kamilfurtak/kamilfurtak.github.io/tree/main/site) as the published output. Content lives in typed data files, pages are lazy-loaded standalone components, metadata is set per route during prerendering, and the whole site ships about 80 kB of JavaScript on first load. Adding a project is a data change; adding a page is one component plus a route.

## Contributions reviewed by other maintainers

- **[bolt.diy #1322](https://github.com/stackblitz-labs/bolt.diy/pull/1322), merged.** Replaced the model selector's static dropdown with search, filtered results, keyboard navigation and focus handling.
- **[Hindsight #3656](https://github.com/vectorize-io/hindsight/pull/3656), merged.** The batch path built a schema from one configuration flag and sent its strictness setting from another. I aligned both decisions with the retain-scoped flag and added tests for both directions of the mismatch.

[Back to my profile](README.md) · [Portfolio](https://furtak.dev/) · [Contact](https://linkedin.com/in/kamilfurtak)
