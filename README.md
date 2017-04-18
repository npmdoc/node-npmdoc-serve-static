# npmdoc-serve-static

#### api documentation for  [serve-static (v1.12.1)](https://github.com/expressjs/serve-static#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-serve-static.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-serve-static) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-serve-static.svg)](https://travis-ci.org/npmdoc/node-npmdoc-serve-static)

#### Serve static files

[![NPM](https://nodei.co/npm/serve-static.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/serve-static)

- [https://npmdoc.github.io/node-npmdoc-serve-static/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-serve-static/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-serve-static/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-serve-static/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-serve-static/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-serve-static/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Douglas Christopher Wilson"
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
            "name": "dougwilson"
        }
    ],
    "name": "serve-static",
    "optionalDependencies": {},
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



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
