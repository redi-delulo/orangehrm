# Sunrise HRM

Sunrise HRM is a web-based human resource management application. This repository contains the PHP backend, installer, and Vue frontend assets.

## Prerequisites

- PHP 7.4 or newer with the extensions listed in `src/composer.json`
- Composer
- Node.js and Yarn 4.x
- A supported SQL database for the full backend installation

## Run the frontend preview

Use this when you only need to preview the Vue client during development.

```bash
cd src/client
yarn install
yarn serve --host 0.0.0.0 --port 8080
```

Open the preview at:

```text
http://localhost:8080
```

If the dev server reports that `web/dist/build` is missing, create the output directory from the repository root and run the command again:

```bash
mkdir -p web/dist
```

## Build frontend assets

```bash
cd src/client
yarn install
yarn build
```

The production assets are written to `web/dist`.

## Run frontend checks

```bash
cd src/client
yarn lint
yarn test:unit
```

## Backend setup

Install PHP dependencies from the backend directory:

```bash
cd src
composer install
```

After dependencies are installed, serve the repository with a PHP-compatible web server whose document root points to the repository `web` directory, then complete setup through the web installer.

## License

GNU General Public License v3.0 or later.
