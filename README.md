# npmtest-co-mocha

#### basic test coverage for  [co-mocha (v1.2.0)](https://github.com/blakeembrey/co-mocha)  [![npm package](https://img.shields.io/npm/v/npmtest-co-mocha.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-co-mocha) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-co-mocha.svg)](https://travis-ci.org/npmtest/node-npmtest-co-mocha)

#### Enable support for generators in Mocha tests

[![NPM](https://nodei.co/npm/co-mocha.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/co-mocha)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-co-mocha/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-co-mocha/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-co-mocha/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-co-mocha/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-co-mocha/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-co-mocha/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-co-mocha/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-co-mocha/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-co-mocha/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-co-mocha/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-co-mocha/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-co-mocha/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-co-mocha/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-co-mocha/build/test-report.html](https://npmtest.github.io/node-npmtest-co-mocha/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-co-mocha/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-co-mocha/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-co-mocha/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-co-mocha/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-co-mocha/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-co-mocha/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-co-mocha/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-co-mocha/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Blake Embrey",
        "url": "http://blakeembrey.me"
    },
    "browser": {
        "path": false
    },
    "bugs": {
        "url": "https://github.com/blakeembrey/co-mocha/issues"
    },
    "dependencies": {
        "co": "^4.0.0",
        "is-generator": "^1.0.1"
    },
    "description": "Enable support for generators in Mocha tests",
    "devDependencies": {
        "browserify": "^14.0.0",
        "chai": "^3.0.0",
        "es6-promise": "^4.0.5",
        "istanbul": "git://github.com/gotwarlost/istanbul.git#harmony",
        "mocha": "^3.1.2",
        "pre-commit": "^1.0.7",
        "regenerator": "^0.9.0",
        "standard": "^8.5.0",
        "testem": "^1.13.0",
        "traceur": "0.0.111"
    },
    "directories": {},
    "dist": {
        "shasum": "d9be35a2a2d16f4b1b0e83f6973401ca4b6660af",
        "tarball": "https://registry.npmjs.org/co-mocha/-/co-mocha-1.2.0.tgz"
    },
    "files": [
        "co-mocha.js",
        "lib/",
        "LICENSE"
    ],
    "gitHead": "629d98852833a98aaee4551f049e22ecfd6685cc",
    "homepage": "https://github.com/blakeembrey/co-mocha",
    "keywords": [
        "co",
        "mocha",
        "harmony",
        "generators"
    ],
    "license": "MIT",
    "main": "lib/co-mocha.js",
    "maintainers": [
        {
            "name": "blakeembrey"
        }
    ],
    "name": "co-mocha",
    "optionalDependencies": {},
    "peerDependencies": {
        "mocha": ">=1.18 <4"
    },
    "repository": {
        "type": "git",
        "url": "git://github.com/blakeembrey/co-mocha.git"
    },
    "scripts": {
        "build": "browserify lib/co-mocha.js -s co-mocha -o co-mocha.js",
        "lint": "standard",
        "test": "npm run lint && npm run build && npm run test-cov",
        "test-cov": "testem ci -l Firefox,Node",
        "test-spec": "mocha --harmony -R spec --require lib/co-mocha.js --bail"
    },
    "standard": {
        "ignore": [
            "coverage/**",
            "node_modules/**",
            "bower_components/**",
            "co-mocha.js"
        ]
    },
    "version": "1.2.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
