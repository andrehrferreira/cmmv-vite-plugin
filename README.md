<p align="center">
  <a href="https://cmmv.io/" target="blank"><img src="https://raw.githubusercontent.com/andrehrferreira/cmmv/main/public/assets/logo_CMMV_negativa.svg" width="300" alt="CMMV Logo" /></a>
</p>
<p align="center">Contract-Model-Model-View (CMMV) <br/> A minimalistic framework for building scalable and modular applications using TypeScript contracts.</p>
<p align="center">
    <a href="https://www.npmjs.com/package/@cmmv/core"><img src="https://img.shields.io/npm/v/@cmmv/core.svg" alt="NPM Version" /></a>
    <a href="https://github.com/andrehrferreira/cmmv/blob/main/LICENSE"><img src="https://img.shields.io/npm/l/@cmmv/core.svg" alt="Package License" /></a>
</p>

<p align="center">
  <a href="https://cmmv.io">Documentation</a> &bull;
  <a href="https://github.com/andrehrferreira/cmmv/issues">Report Issue</a>
</p>

# @cmmv/plugin-vite

``@cmmv/plugin-vite`` is a simple Vite plugin designed for handling .cmmv template files. It enables basic parsing and loading of templates, scripts, and styles, similar to Vue's SFC (Single File Component) format, but with a reduced scope tailored for lightweight component handling.

This plugin was inspired by the [``vite-plugin-vue``](https://github.com/vitejs/vite-plugin-vue/blob/main/packages/plugin-vue) and allows for easy integration of ``.cmmv`` files in Vite projects, focusing on simplicity and performance for component-based development.

## Installation

```bash
$ pnpm add -D @cmmv/plugin-vite
```

## Usage

```typescript
// vite.config.js
import cmmvPlugin from '@cmmv/plugin-vite'

export default {
  plugins: [cmmvPlugin()],
}
```

## Example .cmmv File

```vue
<template>
  <div>{{ message }}</div>
</template>

<script>
export default {
  data() {
    return {
      message: 'Hello CMMV!'
    };
  }
};
</script>

<style>
div {
  color: blue;
}
</style>
```

## Documentation

The complete documentation is available [here](https://cmmv.io).

## Status

- This is pretty new. There are probably bugs and there might still be API changes, so **use at your own risk.** Is it usable though? Very much. Check out the [examples](https://github.com/andrehrferreira/cmmv-reactivity/tree/main/samples) to see what it's capable of.

## Stay in Touch

- Author - [André Ferreira](https://github.com/andrehrferreira)
- Twitter - [@andrehrferreira](https://twitter.com/andrehrferreira)
- Linkdin - [@andrehrf](https://www.linkedin.com/in/andrehrf)
- Youtube - [@Andrehrferreira](https://www.youtube.com/@Andrehrferreira)

## License

CMMV is [MIT licensed](LICENSE).
