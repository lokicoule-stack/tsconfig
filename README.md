<div align="center">
  <img src="https://github.com/lokicoule-stack/tsconfig/blob/main/media/repo-header.svg?raw=true" alt="Lokicoule TypeScript Configuration"  />
</div>

## Installation

```bash
pnpm add -D @lokiverse/tsconfig
```

## Usage

### Base Configuration

```json
{
  "extends": "@lokiverse/tsconfig/base.json"
}
```

### Runtime Configurations

#### Node.js

```json
{
  "extends": "@lokiverse/tsconfig/runtime/node.json"
}
```

#### Browser

```json
{
  "extends": "@lokiverse/tsconfig/runtime/browser.json"
}
```

### Framework Configurations

#### React

```json
{
  "extends": "@lokiverse/tsconfig/frameworks/react.json"
}
```

#### Vite

```json
{
  "extends": "@lokiverse/tsconfig/frameworks/vite.json"
}
```

### Library Presets

#### Base Library

```json
{
  "extends": "@lokiverse/tsconfig/presets/lib-base.json"
}
```

#### Node.js Library

```json
{
  "extends": "@lokiverse/tsconfig/presets/lib-node.json"
}
```

#### Browser Library

```json
{
  "extends": "@lokiverse/tsconfig/presets/lib-browser.json"
}
```

#### React Library

```json
{
  "extends": "@lokiverse/tsconfig/presets/lib-react.json"
}
```
