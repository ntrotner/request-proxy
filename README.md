# Request Proxy

Nx monorepo for request proxy services.

## Prerequisites

- Node.js >= 20
- npm

## Setup

```shell
npm install
```

## How To

### Important Commands

| Command              | Description                    |
| -------------------- | ------------------------------ |
| `npm run lint:fix`   | Lint and fix all projects      |
| `npm run format:fix` | Format and fix all projects    |
| `npm run test`       | Run unit tests on all projects |

### Create a new package

**Non-buildable: source consumed directly, no build step**:

```shell
npx nx g @nx/js:library my-package --directory=packages/my-package --bundler=none --compiler=swc --unitTestRunner=vitest
```

**Buildable**:

```shell
npx nx g @nx/js:library my-package --directory=packages/my-package --bundler=swc --unitTestRunner=vitest
```

## Best Practices

### Commit Message Convention

- `feat(common): add utility function`
- `fix(core): resolve timeout issue`
- `chore(deps): update dependencies`
