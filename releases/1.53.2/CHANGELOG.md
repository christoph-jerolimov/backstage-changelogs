# Backstage Release 1.53.2 changelog

Changes between 1.53.1 and 1.53.2 — 0 added, 0 removed, 3 upgraded, 208 unchanged packages.

## Summary

- [Patch version bumps](#patch-version-bumps): 3 packages

## Table of contents

- [Patch version bumps](#patch-version-bumps)
  - [`@backstage/plugin-catalog-backend` (3.8.1 → 3.8.2)](#backstageplugin-catalog-backend-381--382)
  - [`@backstage/plugin-scaffolder-backend` (4.0.2 → 4.0.3)](#backstageplugin-scaffolder-backend-402--403)
  - [`@backstage/plugin-scaffolder-common` (2.2.1 → 2.2.2)](#backstageplugin-scaffolder-common-221--222)

## Patch version bumps

### `@backstage/plugin-catalog-backend` (3.8.1 → [3.8.2](../../changelogs/@backstage/plugin-catalog-backend.md#382))

_No changelog entries found._

### `@backstage/plugin-scaffolder-backend` (4.0.2 → [4.0.3](../../changelogs/@backstage/plugin-scaffolder-backend.md#403))

#### 4.0.3

##### Patch Changes

- [`4bbc088`](https://github.com/backstage/backstage/commit/4bbc088): Fixed the stale task janitor not being set up by passing the scheduler service to the router.
- [`943687f`](https://github.com/backstage/backstage/commit/943687f): Removed the native addon requirement from scaffolder template rendering. Templates now run through a TypeScript interpreter, and the backend no longer needs the `--no-node-snapshot` Node.js option.
- [`7ca434e`](https://github.com/backstage/backstage/commit/7ca434e): Scaffolder tasks now wait for recovery checkpoint state to be persisted before continuing, preventing later execution from racing ahead of stored recovery state. Restored checkpoints also preserve falsy values without re-running their callbacks.

### `@backstage/plugin-scaffolder-common` (2.2.1 → [2.2.2](../../changelogs/@backstage/plugin-scaffolder-common.md#222))

#### 2.2.2

##### Patch Changes

- [`4e8d763`](https://github.com/backstage/backstage/commit/4e8d763): Migrated tests from MSW v1 to MSW v2.
