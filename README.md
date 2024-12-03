# @lokiverse/tsconfig

<div align="center">
 <img src="https://github.com/lokicoule-stack/tsconfig/blob/main/media/repo-header.svg?raw=true" alt="Lokiverse TypeScript Configuration" />
</div>

<div align="center">

[![npm version](https://img.shields.io/npm/v/@lokiverse/tsconfig.svg)](https://www.npmjs.com/package/@lokiverse/tsconfig)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)

</div>

<div align="center">
  <strong>Composable TypeScript configurations for modern development environments</strong>
</div>

<br />

## 📦 Installation

```bash
pnpm add -D @lokiverse/tsconfig
```

## 🔧 Configuration Types

This package provides several types of configurations that can be combined to create perfect TypeScript setup:

- **Base Configuration**: Core TypeScript settings
- **Runtime Configurations**: Environment-specific settings (Node.js, Browser)
- **Framework Configurations**: Framework-specific settings (React, Vite)
- **Library Presets**: Pre-configured combinations for common use cases

## 📝 Usage

### Base Configuration

The foundation for all configurations:

```json
{
  "extends": "@lokiverse/tsconfig"
}
```

### Runtime Configurations

Runtime configurations should be combined with either the base configuration or framework configurations:

#### Node.js Runtime

```json
{
  "extends": ["@lokiverse/tsconfig", "@lokiverse/tsconfig/runtime/node"]
}
```

#### Browser Runtime

```json
{
  "extends": ["@lokiverse/tsconfig", "@lokiverse/tsconfig/runtime/browser"]
}
```

### Framework Configurations

Framework configurations should be combined with runtime configurations:

#### React with Browser Runtime

```json
{
  "extends": [
    "@lokiverse/tsconfig",
    "@lokiverse/tsconfig/runtime/browser",
    "@lokiverse/tsconfig/frameworks/react"
  ]
}
```

#### Vite with Browser Runtime

```json
{
  "extends": [
    "@lokiverse/tsconfig",
    "@lokiverse/tsconfig/runtime/browser",
    "@lokiverse/tsconfig/frameworks/vite"
  ]
}
```

### Library Presets

Pre-configured combinations for common use cases. These already include the appropriate runtime and framework configurations:

#### Base Library

Foundation for library development:

```json
{
  "extends": "@lokiverse/tsconfig/presets/lib-base"
}
```

#### Node.js Library

Complete setup for Node.js libraries:

```json
{
  "extends": "@lokiverse/tsconfig/presets/lib-node"
}
```

#### Browser Library

Complete setup for browser libraries:

```json
{
  "extends": "@lokiverse/tsconfig/presets/lib-browser"
}
```

#### React Library

Complete setup for React libraries:

```json
{
  "extends": "@lokiverse/tsconfig/presets/lib-react"
}
```

## 🔨 Creating Custom Combinations

### React Application with Node.js Backend

```json
{
  "extends": [
    "@lokiverse/tsconfig",
    "@lokiverse/tsconfig/runtime/node",
    "@lokiverse/tsconfig/frameworks/react"
  ],
  "compilerOptions": {
    // custom options here
  }
}
```

### Vite Application with Browser Features

```json
{
  "extends": [
    "@lokiverse/tsconfig",
    "@lokiverse/tsconfig/runtime/browser",
    "@lokiverse/tsconfig/frameworks/vite"
  ],
  "compilerOptions": {
    // custom options here
  }
}
```
