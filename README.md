# npmdoc-bignum

#### api documentation for  [bignum (v0.12.5)](https://github.com/justmoon/node-bignum#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-bignum.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-bignum) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-bignum.svg)](https://travis-ci.org/npmdoc/node-npmdoc-bignum)

#### Arbitrary-precision integer arithmetic using OpenSSL

[![NPM](https://nodei.co/npm/bignum.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/bignum)

- [https://npmdoc.github.io/node-npmdoc-bignum/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-bignum/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-bignum/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-bignum/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-bignum/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-bignum/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Stefan Thomas",
        "url": "http://www.justmoon.net"
    },
    "binary": {
        "host": "https://rvagg-node.s3-us-west-2.amazonaws.com",
        "module_name": "bignum",
        "module_path": "binding/",
        "remote_path": "./{name}/v{version}"
    },
    "bugs": {
        "url": "https://github.com/justmoon/node-bignum/issues"
    },
    "contributors": [
        {
            "name": "James Halliday"
        },
        {
            "name": "Rod Vagg"
        }
    ],
    "dependencies": {
        "nan": "^2.3.4",
        "node-pre-gyp": "~0.6.28"
    },
    "description": "Arbitrary-precision integer arithmetic using OpenSSL",
    "devDependencies": {
        "aws-sdk": "~2.4.0",
        "put": "~0.0.5",
        "standard": "~7.1.2",
        "tap": "~5.7.2"
    },
    "directories": {},
    "dist": {
        "shasum": "208f2b0e18eb8fd6950917e3718e4cd85cccffcd",
        "tarball": "https://registry.npmjs.org/bignum/-/bignum-0.12.5.tgz"
    },
    "gitHead": "9c3254dbf19c8a56679311e68bba0ae64ef4df7a",
    "homepage": "https://github.com/justmoon/node-bignum#readme",
    "keywords": [
        "openssl",
        "big",
        "bignum",
        "bigint",
        "integer",
        "arithmetic",
        "precision"
    ],
    "license": "MIT",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "bitcoinjs"
        },
        {
            "name": "justmoon"
        },
        {
            "name": "rvagg"
        }
    ],
    "name": "bignum",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/justmoon/node-bignum.git"
    },
    "scripts": {
        "install": "node-pre-gyp install --fallback-to-build",
        "test": "standard && tap test/*.js"
    },
    "version": "0.12.5"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
