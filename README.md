# DigitalEyeStrain

An early-stage Vue 3 web app intended to help people reduce digital eye strain, with planned pages for an eye-break timer, tips and settings. Only the application shell exists so far; the feature pages were never built.

## Stack

- Vue 3 (Composition API, `<script setup>`)
- Vue Router 4
- Vite 6
- ESLint and Prettier

## Running

The app lives in the `DigitalEyeStrain/` subfolder:

```sh
cd DigitalEyeStrain
npm install
npm run dev
```

Other scripts: `npm run build`, `npm run preview`, `npm run lint`, `npm run format`.

## Project layout

- `DigitalEyeStrain/src/App.vue` - navigation bar (Home, Eye Timer, Tips, Settings), footer and base styles
- `DigitalEyeStrain/src/router/index.js` - router with a single home route
- `DigitalEyeStrain/src/views/MainView.vue` - placeholder home view
- `src/App.vue` - an unused placeholder at the repository root

## Status

Work in progress, mostly a scaffold. The navigation links for Eye Timer, Tips and Settings do not have routes or pages yet, and there is no timer logic. A related static site for the same idea is in the DigitalEyeStrainWeb repository.
