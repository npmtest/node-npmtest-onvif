# npmtest-onvif

#### basic test coverage for  [onvif (v0.5.3)](https://github.com/agsh/onvif#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-onvif.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-onvif) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-onvif.svg)](https://travis-ci.org/npmtest/node-npmtest-onvif)

#### Client to ONVIF NVT devices Profile S: cameras

[![NPM](https://nodei.co/npm/onvif.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/onvif)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-onvif/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-onvif/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-onvif/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-onvif/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-onvif/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-onvif/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-onvif/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-onvif/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-onvif/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-onvif/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-onvif/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-onvif/build/test-report.html](https://npmtest.github.io/node-npmtest-onvif/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-onvif/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-onvif/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-onvif/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-onvif/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-onvif/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-onvif/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-onvif/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-onvif/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Andrew D.Laptev"
    },
    "bugs": {
        "url": "https://github.com/agsh/onvif/issues"
    },
    "dependencies": {
        "xml2js": "^0.4"
    },
    "description": "Client to ONVIF NVT devices Profile S: cameras",
    "devDependencies": {
        "coffee-script": "^1.9.3",
        "coveralls": ">=2.11.2",
        "dot": "^1.0.3",
        "istanbul": ">=0.3.5",
        "jscs": "^1.13.1",
        "jsdoc": "^3.3.0",
        "jshint": "^2.7.0",
        "keypress": "^0.2.1",
        "mocha": ">=2.1.0",
        "mocha-lcov-reporter": "0.0.1",
        "nimble": "^0.0.2"
    },
    "directories": {},
    "dist": {
        "shasum": "39e284065cf1039f8e550c19eb27ec0384c5acb3",
        "tarball": "https://registry.npmjs.org/onvif/-/onvif-0.5.3.tgz"
    },
    "engines": {
        "node": ">=0.12"
    },
    "gitHead": "79461001461917ad5a9452c8c8b6332e477dd0bb",
    "homepage": "https://github.com/agsh/onvif#readme",
    "keywords": [
        "onvif",
        "video",
        "PTZ",
        "camera",
        "RTSP"
    ],
    "license": "MIT",
    "main": "lib/onvif.js",
    "maintainers": [
        {
            "name": "agsh"
        }
    ],
    "name": "onvif",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/agsh/onvif.git"
    },
    "scripts": {
        "coffee-tests": "coffee -c test/*.coffee",
        "gh-pages": "jsdoc ./lib/*.js --readme ./README.md --destination ./",
        "jscs": "jscs lib/*.js",
        "jsdoc": "jsdoc ./lib/*.js --readme ./README.md --destination ./docs",
        "lint": "jshint lib/*.js",
        "pretest": "npm run lint && npm run jscs && npm run coffee-tests",
        "test": "istanbul cover _mocha",
        "test-coveralls": "istanbul cover _mocha --report lcovonly -- -R spec && cat ./coverage/lcov.info | coveralls && rm -rf ./coverage",
        "test-on-travis": "npm run pretest && istanbul cover _mocha --report lcovonly",
        "upload-to-coveralls": "cat ./coverage/lcov.info | coveralls"
    },
    "version": "0.5.3",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
