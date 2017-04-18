# npmdoc-dnode

#### api documentation for  [dnode (v1.2.2)](https://github.com/substack/dnode#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-dnode.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-dnode) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-dnode.svg)](https://travis-ci.org/npmdoc/node-npmdoc-dnode)

#### freestyle rpc

[![NPM](https://nodei.co/npm/dnode.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/dnode)

- [https://npmdoc.github.io/node-npmdoc-dnode/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-dnode/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-dnode/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-dnode/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-dnode/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-dnode/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "James Halliday",
        "url": "http://substack.net"
    },
    "browserify": "browser.js",
    "bugs": {
        "url": "https://github.com/substack/dnode/issues"
    },
    "dependencies": {
        "dnode-protocol": "~0.2.2",
        "jsonify": "~0.0.0",
        "weak": "^1.0.0"
    },
    "description": "freestyle rpc",
    "devDependencies": {
        "tape": "~2.3.2"
    },
    "directories": {},
    "dist": {
        "shasum": "4ac3cfe26e292b3b39b8258ae7d94edc58132efa",
        "tarball": "https://registry.npmjs.org/dnode/-/dnode-1.2.2.tgz"
    },
    "engine": {
        "node": ">=0.6.0"
    },
    "gitHead": "32e8a7e36f4603672b17fa4b0fbecc05c66022df",
    "homepage": "https://github.com/substack/dnode#readme",
    "keywords": [
        "rpc",
        "callbacks"
    ],
    "main": "./index.js",
    "maintainers": [
        {
            "name": "substack"
        },
        {
            "name": "seethroughtrees"
        }
    ],
    "name": "dnode",
    "optionalDependencies": {
        "weak": "^1.0.0"
    },
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/substack/dnode.git"
    },
    "scripts": {
        "test": "tape test/*.js test/server/*.js"
    },
    "testling": {
        "files": "test/*.js",
        "browsers": [
            "ie/6..latest",
            "chrome/10",
            "chrome/latest",
            "chrome/canary",
            "firefox/10",
            "firefox/latest",
            "firefox/nightly",
            "safari/latest",
            "opera/11.0..latest",
            "iphone/6",
            "ipad/6",
            "android-browser/latest"
        ]
    },
    "version": "1.2.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
