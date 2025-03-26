# VoltScript - a language grammar for [highlight.js](https://highlightjs.org/)

VoltScript is a [BASIC](https://en.wikipedia.org/wiki/BASIC) scripting language evolved from LotusScript®, which was developed for the Lotus Software family of products. The language has been extended for use with HCL Volt MX Go, as a server-side scripting language running within the Volt MX Go Foundry middleware layer.

## Usage

Simply include the Highlight.js library in your webpage or Node app, then load this module.

### Static website or simple usage

Simply load the module after loading Highlight.js. You'll use the minified version found in the `dist` directory. This module is just a CDN build of the language, so it will register itself as the Javascript is loaded.

```html
<script type="text/javascript" src="/path/to/highlight.min.js"></script>
<script type="text/javascript" charset="UTF-8"
  src="/path/to/highlightjs-voltscript/dist/voltscript.min.js"></script>
<script type="text/javascript">
  hljs.highlightAll();
</script>
```

### With Node or another build system

If you're using Node / Webpack / Rollup / Browserify, etc, simply require the language module, then register it with Highlight.js.

```javascript
var hljs = require('highlightjs');
var hljsVoltScript = require('highlightjs-voltscript');

hljs.registerLanguage("voltscript", hljsVoltScript);
hljs.highlightAll();
```

## License

This Highlight.js definition is released under the Apache License. See [LICENSE.md][1] file for details.

### Author

Chester Moses <chester-moses@hcl-software.com>

## Links

- The official site for the Highlight.js library is <https://highlightjs.org/>.
- The Highlight.js GitHub project: <https://github.com/highlightjs/highlight.js>
- Learn more about VoltScript: <https://help.hcl-software.com/docs/voltscript/early-access/index.html>

[1]: https://github.com/HCL-TECH-SOFTWARE/highlightjs-voltscript/blob/master/LICENSE.md
