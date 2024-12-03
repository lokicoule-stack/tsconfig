# @lokiverse/tsconfig

## 0.2.0

### Minor Changes

- b77797f: docs: update README.md with new configuration examples and details

  - Added badges and header image
  - Updated installation and configuration types sections
  - Provided detailed usage examples for base, runtime, and framework configurations
  - Added sections for library presets and creating custom combinations

  feat: add exports field to package.json and update framework configs

  - Added exports field to package.json with various paths
  - Removed extends field from react.json and vite.json configurations

## 0.1.1

### Patch Changes

- 956b342: fix: correct tsconfig paths in README.md

  - Updated tsconfig paths from @kumikojs to @lokiverse in README.md

## 0.1.0

### Minor Changes

- e2e9720: Initial release:

  - Added base configuration in `base.json`
  - Added React-specific configuration in `frameworks/react.json`
  - Added Vite-specific configuration in `frameworks/vite.json`
  - Added library base configuration in `presets/lib-base.json`
  - Added browser library configuration in `presets/lib-browser.json`
  - Added Node.js library configuration in `presets/lib-node.json`
  - Added React library configuration in `presets/lib-react.json`
  - Added browser runtime configuration in `runtime/browser.json`
  - Added Node.js runtime configuration in `runtime/node.json`
