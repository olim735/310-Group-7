# Favicon and Logo Update

## Branch

The work was completed on `feature/favicon`.

## Changes

- Added the supplied Pipeline beaver logo to `src/assets/pipelinelogo.png`.
- Added a public favicon copy at `public/favicon.png` so browsers can load it from `/favicon.png`.
- Updated `index.html` to use the PNG favicon instead of `public/favicon.svg`.
- Updated `src/components/Logo.jsx` to display the new beaver image instead of the previous CSS-generated white ring and grey dot.
- The shared `Logo` component carries this change to the sidebar, authentication card, and route-loading screen.
- Removed only the generated front-facing mascot asset, `src/assets/beaverFront.png`.
- Left the original `src/assets/beaver.png`, `src/assets/beaverArms.png`, and unused `src/assets/logo.png` assets unchanged.

## Dependency Note

The favicon work does not require new packages. A local `npm install` changed the locked `nanoid` patch version in `package-lock.json`; that dependency change is unrelated to this feature and does not need to be included with the favicon update.

The dashboard uses the existing `@dnd-kit` dependencies for drag-and-drop behavior. Those packages must be installed locally before the dashboard can build or run.
