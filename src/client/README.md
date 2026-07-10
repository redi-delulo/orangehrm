# Sunrise HRM Client

Vue frontend for Sunrise HRM.

## Prerequisites

- Node.js
- Yarn 4.x

## Install dependencies

```bash
yarn install
```

## Start development server

```bash
yarn serve --host 0.0.0.0 --port 8080
```

Open `http://localhost:8080` in your browser or workspace preview.

If the dev server reports that `web/dist/build` is missing, run this from the repository root and restart the dev server:

```bash
mkdir -p web/dist
```

## Build production assets

```bash
yarn build
```

Assets are emitted to `../../web/dist`.

## Checks

```bash
yarn lint
yarn test:unit
```
