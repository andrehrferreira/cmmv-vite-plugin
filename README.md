<p align="center">
  <a href="https://cmmv.io/" target="blank"><img src="https://raw.githubusercontent.com/andrehrferreira/docs.cmmv.io/main/public/assets/logo_CMMV2_icon.png" width="300" alt="CMMV Logo" /></a>
</p>
<p align="center">Contract-Model-Model-View (CMMV) <br/> Building scalable and modular applications using contracts.</p>
<p align="center">
    <a href="https://www.npmjs.com/package/@cmmv/core"><img src="https://img.shields.io/npm/v/@cmmv/core.svg" alt="NPM Version" /></a>
    <a href="https://github.com/andrehrferreira/cmmv/blob/main/LICENSE"><img src="https://img.shields.io/npm/l/@cmmv/core.svg" alt="Package License" /></a>
</p>

<p align="center">
  <a href="https://cmmv.io">Documentation</a> &bull;
  <a href="https://github.com/andrehrferreira/vite-plugin-cmmv/issues">Report Issue</a>
</p>

# Description

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