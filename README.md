# MCFunction - a language grammar for highlight.js

## Usage

Simply include the Highlight.js library in your webpage or Node app, then load this module.

### Static website or simple usage

Simply load the module after loading Highlight.js. You'll use the minified version found in the `dist` directory. This module is just a CDN build of the language, so it will register itself as the Javascript is loaded.

```html
<script type="text/javascript" src="/path/to/highlight.min.js"></script>
<script type="text/javascript" charset="UTF-8"
  src="/path/to/highlightjs-mcfunction/dist/mcfunction.min.js"></script>
<script type="text/javascript">
  hljs.initHighlightingOnLoad();
</script>
```

### With Node or another build system

If you're using Node / Webpack / Rollup / Browserify, etc, simply require the language module, then register it with Highlight.js.

```javascript
var hljs = require('highlightjs');
var hljsMCFunction = require('highlightjs-mcfunction');

hljs.registerLanguage("mcfunction", hljsMCFunction);
hljs.initHighlightingOnLoad();
```


## License

This project is released under the MIT License. See [LICENSE][1] file for details.

## Links

- The official site for the Highlight.js library is <https://highlightjs.org/>.
- The Highlight.js GitHub project: <https://github.com/highlightjs/highlight.js>.
- Learn more about MCFunction: <https://minecraft.gamepedia.com/Function_(Java_Edition)>.

[1]: https://github.com/TheFireBlast/highlightjs-mcfunction/blob/master/LICENSE
