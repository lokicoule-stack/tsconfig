# @lokiverse/tsconfig

<div align="center">
 <img src="https://github.com/lokicoule-stack/tsconfig/blob/main/media/repo-header.svg?raw=true" alt="Lokiverse TypeScript Configuration" />
</div>

<div align="center">

[![npm version](https://img.shields.io/npm/v/@lokiverse/tsconfig.svg)](https://www.npmjs.com/package/@lokiverse/tsconfig)

Composable TypeScript configurations for modern development.

</div>

## Quick Start

```bash
npm install -D @lokiverse/tsconfig
```

**tsconfig.json**

```json
{
  "extends": "@lokiverse/tsconfig/presets/lib-universal"
}
```

## Library Presets

| Preset          | Target          | Module Resolution | Use Case            |
| --------------- | --------------- | ----------------- | ------------------- |
| `lib-universal` | Node.js + Bun   | Bundler           | Universal libraries |
| `lib-node`      | Node.js         | NodeNext          | Node.js libraries   |
| `lib-browser`   | Browser         | Bundler           | Browser libraries   |
| `lib-react`     | Browser + React | Bundler           | React libraries     |

### Universal Library (Node.js + Bun)

```json
{
  "extends": "@lokiverse/tsconfig/presets/lib-universal"
}
```

### Node.js Library

```json
{
  "extends": "@lokiverse/tsconfig/presets/lib-node"
}
```

### Browser Library

```json
{
  "extends": "@lokiverse/tsconfig/presets/lib-browser"
}
```

### React Library

```json
{
  "extends": "@lokiverse/tsconfig/presets/lib-react"
}
```

## Custom Configurations

### Composable Configs

Build custom configs by combining base, runtime, and framework configs.

**React App with Node.js**

```json
{
  "extends": [
    "@lokiverse/tsconfig",
    "@lokiverse/tsconfig/runtimes/node",
    "@lokiverse/tsconfig/frameworks/react"
  ]
}
```

**Vite App**

```json
{
  "extends": [
    "@lokiverse/tsconfig",
    "@lokiverse/tsconfig/runtimes/browser",
    "@lokiverse/tsconfig/frameworks/vite"
  ]
}
```

## Available Configs

### Base

- `@lokiverse/tsconfig` - Core TypeScript settings

### Runtimes

- `@lokiverse/tsconfig/runtimes/node` - Node.js environment
- `@lokiverse/tsconfig/runtimes/browser` - Browser environment

### Frameworks

- `@lokiverse/tsconfig/frameworks/react` - React support
- `@lokiverse/tsconfig/frameworks/vite` - Vite support

### Library Presets

- `@lokiverse/tsconfig/presets/lib-base` - Base library config
- `@lokiverse/tsconfig/presets/lib-universal` - Node.js + Bun
- `@lokiverse/tsconfig/presets/lib-node` - Node.js only
- `@lokiverse/tsconfig/presets/lib-browser` - Browser only
- `@lokiverse/tsconfig/presets/lib-react` - React libraries

## What's Included

- Strict type checking enabled
- Source maps and declarations
- Modern ES2022 target
- Optimized for bundlers
- Incremental compilation support

## License

MIT
