# test coverage for  [zombie (v5.0.5)](https://www.npmjs.com/package/zombie)  [![npm package](https://img.shields.io/npm/v/npmtest-zombie.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-zombie) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-zombie.svg)](https://travis-ci.org/npmtest/node-npmtest-zombie)
#### Insanely fast, full-stack, headless browser testing using Node.js

[![NPM](https://nodei.co/npm/zombie.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/zombie)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-zombie/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-zombie/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-zombie/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-zombie/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-zombie/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-zombie/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-zombie/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-zombie/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-zombie/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-zombie/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-zombie/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-zombie/build/test-report.html](https://npmtest.github.io/node-npmtest-zombie/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-zombie/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-zombie/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-zombie/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-zombie/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-zombie/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-zombie/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-zombie/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-zombie/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Assaf Arkin",
        "url": "http://labnotes.org/"
    },
    "bugs": {
        "url": "http://github.com/assaf/zombie/issues"
    },
    "contributors": [
        {
            "name": "Bob Lail",
            "url": "http://boblail.tumblr.com/"
        },
        {
            "name": "Brian McDaniel",
            "url": "https://github.com/brianmcd"
        },
        {
            "name": "Damian Janowski"
        },
        {
            "name": "José Valim",
            "url": "http://blog.plataformatec.com.br/"
        },
        {
            "name": "Matt Lavin",
            "url": "https://github.com/mdlavin"
        }
    ],
    "dependencies": {
        "babel-runtime": "5.8.29",
        "bluebird": "^3.0",
        "debug": "^2.2",
        "eventsource": "^0.1.6",
        "iconv-lite": "^0.4.13",
        "jsdom": "^7.2.2",
        "lodash": "^3.10.1",
        "mime": "^1.3.4",
        "ms": "^0.7.1",
        "request": "^2.65.0",
        "tough-cookie": "^2.2.0",
        "ws": "^1.0.1"
    },
    "description": "Insanely fast, full-stack, headless browser testing using Node.js",
    "devDependencies": {
        "babel": "5.8.29",
        "babel-eslint": "^4.0.10",
        "body-parser": "^1.13.3",
        "cookie-parser": "^1.3.5",
        "del": "^2.0.2",
        "eslint": "^1.7.3",
        "express": "^4.13.3",
        "gulp": "^3.9.0",
        "gulp-babel": "^5.3.0",
        "gulp-eslint": "^1.0.0",
        "gulp-exec": "^2.1.2",
        "gulp-notify": "^2.0.1",
        "gulp-sourcemaps": "^1.5.2",
        "gulp-util": "^3.0.7",
        "mocha": "^2.2.5",
        "morgan": "^1.6.1",
        "multiparty": "^4.1.2",
        "replay": "^2.1.2",
        "requirejs": "^2.1.20"
    },
    "directories": {},
    "dist": {
        "shasum": "69da3fa34959ec0f066746267803197a828485c3",
        "tarball": "https://registry.npmjs.org/zombie/-/zombie-5.0.5.tgz"
    },
    "engines": {
        "node": ">=4.0.0"
    },
    "gitHead": "99d05d30720ab709ff1683d98bec04b07842a272",
    "homepage": "https://www.npmjs.com/package/zombie",
    "keywords": [
        "test",
        "tests",
        "testing",
        "TDD",
        "spec",
        "specs",
        "BDD",
        "headless",
        "browser",
        "html",
        "html5",
        "dom",
        "css",
        "javascript",
        "integration",
        "ajax",
        "full-stack",
        "DSL"
    ],
    "license": "MIT",
    "main": "lib",
    "maintainers": [
        {
            "name": "assaf"
        },
        {
            "name": "mdlavin"
        }
    ],
    "name": "zombie",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/assaf/zombie.git"
    },
    "scripts": {
        "build": "gulp build",
        "postpublish": "git push",
        "prepublish": "npm test && gulp build",
        "test": "gulp lint && mocha"
    },
    "version": "5.0.5"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
