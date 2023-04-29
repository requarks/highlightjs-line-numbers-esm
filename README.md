# highlightjs-line-numbers-esm

Fork of the [Highlight.js Line Numbers](https://www.npmjs.com/package/highlightjs-line-numbers.js) plugin for [Highlight.js](https://github.com/highlightjs/highlight.js) line refactored for ESM.

## Install

Copy the `src/highlightjs-line-numbers.js` file into your project.

## Usage

Import both Highlight.js and the `highlightjs-line-numbers.js` file, then register the plugin:

```js
// Import both libraries
import hljs from 'highlight.js'
import { registerHljsLineNumbers, injectHljsLineNumbersCss } from './src/highlightjs-line-numbers.js'

// Register the plugin
registerHljsLineNumbers(hljs)

// Optionally inject the default CSS for line numbers
injectHljsLineNumbersCss()
```

- `registerHljsLineNumbers(hljs)` requires the `hljs` instance to be passed as its sole parameter.
- `injectHljsLineNumbersCss()` will inject the base CSS for this plugin.

You can then call the `hljs.lineNumbersBlock()`, `hljs.initLineNumbersOnLoad()` and `hljs.lineNumbersValue()` methods as needed.

For more info, read the [original plugin documentation](https://www.npmjs.com/package/highlightjs-line-numbers.js).
