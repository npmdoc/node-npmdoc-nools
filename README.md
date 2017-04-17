# api documentation for  [nools (v0.4.4)](http://c2fo.github.com/nools)  [![npm package](https://img.shields.io/npm/v/npmdoc-nools.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-nools) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-nools.svg)](https://travis-ci.org/npmdoc/node-npmdoc-nools)
#### A rules engine for node

[![NPM](https://nodei.co/npm/nools.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/nools)

- [https://npmdoc.github.io/node-npmdoc-nools/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-nools/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-nools/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-nools/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-nools/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-nools/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Doug Martin",
        "url": "http://c2fo.com"
    },
    "bin": {
        "nools": "./bin/nools"
    },
    "bugs": {
        "url": "https://github.com/C2FO/nools/issues"
    },
    "dependencies": {
        "arguments-extended": "~0.0.3",
        "array-extended": "~0.0.4",
        "commander": "~1.1.1",
        "date-extended": "~0.0.3",
        "declare.js": "~0.0.3",
        "extended": "~0.0.3",
        "function-extended": "~0.0.3",
        "ht": "~0.0.2",
        "is-extended": "~0.0.4",
        "leafy": "~0.0.3",
        "object-extended": "~0.0.3",
        "promise-extended": "~0.0.3",
        "string-extended": "~0.0.3",
        "uglify-js": "~2.4.24"
    },
    "description": "A rules engine for node",
    "devDependencies": {
        "coddoc": "0.0.3",
        "grunt": "~0.4.1",
        "grunt-browserify": "1.2.4",
        "grunt-contrib-jshint": "~0.5.3",
        "grunt-contrib-uglify": "~0.2.0",
        "grunt-exec": "^0.4.5",
        "grunt-it": "~0.3.0",
        "it": "~0.2.0",
        "jison": "~0.4.17"
    },
    "directories": {
        "lib": "lib"
    },
    "dist": {
        "shasum": "d9f70671ee2926bd24bb62a8c605cae209199a86",
        "tarball": "https://registry.npmjs.org/nools/-/nools-0.4.4.tgz"
    },
    "engines": {
        "node": ">= 0.6.1"
    },
    "gitHead": "019cdc7d71a80a9c9f1c2dbd63b78a2e311a380b",
    "homepage": "http://c2fo.github.com/nools",
    "keywords": [
        "rules",
        "flow",
        "rules engine",
        "rools",
        "drools",
        "async",
        "flow control"
    ],
    "main": "index.js",
    "maintainers": [
        {
            "name": "damartin"
        },
        {
            "name": "devside"
        }
    ],
    "name": "nools",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/C2FO/nools.git"
    },
    "scripts": {
        "create-doc": "rm -rf docs/* && coddoc -d ./lib -f multi-html",
        "test": "it -r spec"
    },
    "testling": {
        "files": "test/browserling.js",
        "browsers": [
            "ie/8..latest",
            "chrome/20..latest",
            "firefox/14..latest",
            "safari/latest",
            "iphone/6",
            "ipad/6"
        ]
    },
    "version": "0.4.4"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
