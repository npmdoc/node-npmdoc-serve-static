# api documentation for  [serve-static (v1.12.1)](https://github.com/expressjs/serve-static#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-serve-static.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-serve-static) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-serve-static.svg)](https://travis-ci.org/npmdoc/node-npmdoc-serve-static)
#### Serve static files

[![NPM](https://nodei.co/npm/serve-static.png?downloads=true)](https://www.npmjs.com/package/serve-static)

[![apidoc](https://npmdoc.github.io/node-npmdoc-serve-static/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-serve-static_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-serve-static/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-serve-static/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Douglas Christopher Wilson",
        "email": "doug@somethingdoug.com"
    },
    "bugs": {
        "url": "https://github.com/expressjs/serve-static/issues"
    },
    "dependencies": {
        "encodeurl": "~1.0.1",
        "escape-html": "~1.0.3",
        "parseurl": "~1.3.1",
        "send": "0.15.1"
    },
    "description": "Serve static files",
    "devDependencies": {
        "eslint": "3.17.0",
        "eslint-config-standard": "7.0.0",
        "eslint-plugin-markdown": "1.0.0-beta.4",
        "eslint-plugin-promise": "3.5.0",
        "eslint-plugin-standard": "2.1.1",
        "istanbul": "0.4.5",
        "mocha": "2.5.3",
        "supertest": "1.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "7443a965e3ced647aceb5639fa06bf4d1bbe0039",
        "tarball": "https://registry.npmjs.org/serve-static/-/serve-static-1.12.1.tgz"
    },
    "engines": {
        "node": ">= 0.8.0"
    },
    "files": [
        "LICENSE",
        "HISTORY.md",
        "index.js"
    ],
    "gitHead": "3e6e778fcf6c88dcf659b8f1d5f06be2eebbe2db",
    "homepage": "https://github.com/expressjs/serve-static#readme",
    "license": "MIT",
    "maintainers": [
        {
            "name": "dougwilson",
            "email": "doug@somethingdoug.com"
        }
    ],
    "name": "serve-static",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/expressjs/serve-static.git"
    },
    "scripts": {
        "lint": "eslint --plugin markdown --ext js,md .",
        "test": "mocha --reporter spec --bail --check-leaks test/",
        "test-ci": "istanbul cover node_modules/mocha/bin/_mocha --report lcovonly -- --reporter spec --check-leaks test/",
        "test-cov": "istanbul cover node_modules/mocha/bin/_mocha -- --reporter dot --check-leaks test/"
    },
    "version": "1.12.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module serve-static](#apidoc.module.serve-static)
1.  [function <span class="apidocSignatureSpan">serve-static.</span>mime.Mime ()](#apidoc.element.serve-static.mime.Mime)
1.  object <span class="apidocSignatureSpan">serve-static.</span>mime
1.  object <span class="apidocSignatureSpan">serve-static.</span>mime.Mime.prototype
1.  object <span class="apidocSignatureSpan">serve-static.</span>mime.charsets

#### [module serve-static.mime](#apidoc.module.serve-static.mime)
1.  [function <span class="apidocSignatureSpan">serve-static.mime.</span>Mime ()](#apidoc.element.serve-static.mime.Mime)
1.  object <span class="apidocSignatureSpan">serve-static.mime.</span>charsets
1.  object <span class="apidocSignatureSpan">serve-static.mime.</span>extensions
1.  object <span class="apidocSignatureSpan">serve-static.mime.</span>types
1.  string <span class="apidocSignatureSpan">serve-static.mime.</span>default_type

#### [module serve-static.mime.Mime](#apidoc.module.serve-static.mime.Mime)
1.  [function <span class="apidocSignatureSpan">serve-static.mime.</span>Mime ()](#apidoc.element.serve-static.mime.Mime.Mime)

#### [module serve-static.mime.Mime.prototype](#apidoc.module.serve-static.mime.Mime.prototype)
1.  [function <span class="apidocSignatureSpan">serve-static.mime.Mime.prototype.</span>define (map)](#apidoc.element.serve-static.mime.Mime.prototype.define)
1.  [function <span class="apidocSignatureSpan">serve-static.mime.Mime.prototype.</span>extension (mimeType)](#apidoc.element.serve-static.mime.Mime.prototype.extension)
1.  [function <span class="apidocSignatureSpan">serve-static.mime.Mime.prototype.</span>load (file)](#apidoc.element.serve-static.mime.Mime.prototype.load)
1.  [function <span class="apidocSignatureSpan">serve-static.mime.Mime.prototype.</span>lookup (path, fallback)](#apidoc.element.serve-static.mime.Mime.prototype.lookup)

#### [module serve-static.mime.charsets](#apidoc.module.serve-static.mime.charsets)
1.  [function <span class="apidocSignatureSpan">serve-static.mime.charsets.</span>lookup (mimeType, fallback)](#apidoc.element.serve-static.mime.charsets.lookup)



# <a name="apidoc.module.serve-static"></a>[module serve-static](#apidoc.module.serve-static)

#### <a name="apidoc.element.serve-static.mime.Mime"></a>[function <span class="apidocSignatureSpan">serve-static.</span>mime.Mime ()](#apidoc.element.serve-static.mime.Mime)
- description and source-code
```javascript
function Mime() {
  // Map of extension -> mime type
  this.types = Object.create(null);

  // Map of mime type -> extension
  this.extensions = Object.create(null);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.serve-static.mime"></a>[module serve-static.mime](#apidoc.module.serve-static.mime)

#### <a name="apidoc.element.serve-static.mime.Mime"></a>[function <span class="apidocSignatureSpan">serve-static.mime.</span>Mime ()](#apidoc.element.serve-static.mime.Mime)
- description and source-code
```javascript
function Mime() {
  // Map of extension -> mime type
  this.types = Object.create(null);

  // Map of mime type -> extension
  this.extensions = Object.create(null);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.serve-static.mime.Mime"></a>[module serve-static.mime.Mime](#apidoc.module.serve-static.mime.Mime)

#### <a name="apidoc.element.serve-static.mime.Mime.Mime"></a>[function <span class="apidocSignatureSpan">serve-static.mime.</span>Mime ()](#apidoc.element.serve-static.mime.Mime.Mime)
- description and source-code
```javascript
function Mime() {
  // Map of extension -> mime type
  this.types = Object.create(null);

  // Map of mime type -> extension
  this.extensions = Object.create(null);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.serve-static.mime.Mime.prototype"></a>[module serve-static.mime.Mime.prototype](#apidoc.module.serve-static.mime.Mime.prototype)

#### <a name="apidoc.element.serve-static.mime.Mime.prototype.define"></a>[function <span class="apidocSignatureSpan">serve-static.mime.Mime.prototype.</span>define (map)](#apidoc.element.serve-static.mime.Mime.prototype.define)
- description and source-code
```javascript
define = function (map) {
  for (var type in map) {
    var exts = map[type];
    for (var i = 0; i < exts.length; i++) {
      if (process.env.DEBUG_MIME && this.types[exts]) {
        console.warn(this._loading.replace(/.*\//, ''), 'changes "' + exts[i] + '" extension type from ' +
          this.types[exts] + ' to ' + type);
      }

      this.types[exts[i]] = type;
    }

    // Default extension is the first one we encounter
    if (!this.extensions[type]) {
      this.extensions[type] = exts[0];
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.serve-static.mime.Mime.prototype.extension"></a>[function <span class="apidocSignatureSpan">serve-static.mime.Mime.prototype.</span>extension (mimeType)](#apidoc.element.serve-static.mime.Mime.prototype.extension)
- description and source-code
```javascript
extension = function (mimeType) {
  var type = mimeType.match(/^\s*([^;\s]*)(?:;|\s|$)/)[1].toLowerCase();
  return this.extensions[type];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.serve-static.mime.Mime.prototype.load"></a>[function <span class="apidocSignatureSpan">serve-static.mime.Mime.prototype.</span>load (file)](#apidoc.element.serve-static.mime.Mime.prototype.load)
- description and source-code
```javascript
load = function (file) {
  this._loading = file;
  // Read file and split into lines
  var map = {},
      content = fs.readFileSync(file, 'ascii'),
      lines = content.split(/[\r\n]+/);

  lines.forEach(function(line) {
    // Clean up whitespace/comments, and split into fields
    var fields = line.replace(/\s*#.*|^\s*|\s*$/g, '').split(/\s+/);
    map[fields.shift()] = fields;
  });

  this.define(map);

  this._loading = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.serve-static.mime.Mime.prototype.lookup"></a>[function <span class="apidocSignatureSpan">serve-static.mime.Mime.prototype.</span>lookup (path, fallback)](#apidoc.element.serve-static.mime.Mime.prototype.lookup)
- description and source-code
```javascript
lookup = function (path, fallback) {
  var ext = path.replace(/.*[\.\/\\]/, '').toLowerCase();

  return this.types[ext] || fallback || this.default_type;
}
```
- example usage
```shell
...
  maxAge: '1d',
  setHeaders: setCustomCacheControl
}))

app.listen(3000)

function setCustomCacheControl (res, path) {
  if (serveStatic.mime.lookup(path) === 'text/html') {
    // Custom Cache-Control for HTML files
    res.setHeader('Cache-Control', 'public, max-age=0')
  }
}
'''

## License
...
```



# <a name="apidoc.module.serve-static.mime.charsets"></a>[module serve-static.mime.charsets](#apidoc.module.serve-static.mime.charsets)

#### <a name="apidoc.element.serve-static.mime.charsets.lookup"></a>[function <span class="apidocSignatureSpan">serve-static.mime.charsets.</span>lookup (mimeType, fallback)](#apidoc.element.serve-static.mime.charsets.lookup)
- description and source-code
```javascript
lookup = function (mimeType, fallback) {
  // Assume text types are utf8
  return (/^text\//).test(mimeType) ? 'UTF-8' : fallback;
}
```
- example usage
```shell
...
  maxAge: '1d',
  setHeaders: setCustomCacheControl
}))

app.listen(3000)

function setCustomCacheControl (res, path) {
  if (serveStatic.mime.lookup(path) === 'text/html') {
    // Custom Cache-Control for HTML files
    res.setHeader('Cache-Control', 'public, max-age=0')
  }
}
'''

## License
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
