# npmtest-sass-loader

#### basic test coverage for  [sass-loader (v6.0.3)](https://github.com/webpack-contrib/sass-loader#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-sass-loader.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-sass-loader) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-sass-loader.svg)](https://travis-ci.org/npmtest/node-npmtest-sass-loader)

#### Sass loader for webpack

[![NPM](https://nodei.co/npm/sass-loader.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/sass-loader)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-sass-loader/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-sass-loader/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-sass-loader/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-sass-loader/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-sass-loader/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-sass-loader/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-sass-loader/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-sass-loader/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-sass-loader/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-sass-loader/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-sass-loader/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-sass-loader/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-sass-loader/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-sass-loader/build/test-report.html](https://npmtest.github.io/node-npmtest-sass-loader/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-sass-loader/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-sass-loader/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-sass-loader/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-sass-loader/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-sass-loader/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-sass-loader/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-sass-loader/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-sass-loader/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "J. Tangelder"
    },
    "bugs": {
        "url": "https://github.com/webpack-contrib/sass-loader/issues"
    },
    "dependencies": {
        "async": "^2.1.5",
        "clone-deep": "^0.2.4",
        "loader-utils": "^1.0.1",
        "lodash.tail": "^4.1.1",
        "pify": "^2.3.0"
    },
    "description": "Sass loader for webpack",
    "devDependencies": {
        "bootstrap-sass": "^3.3.5",
        "css-loader": "^0.26.1",
        "eslint": "^3.16.0",
        "eslint-config-peerigon": "^9.0.0",
        "eslint-plugin-jsdoc": "^2.4.0",
        "file-loader": "^0.10.0",
        "mocha": "^3.0.2",
        "node-sass": "^4.5.0",
        "nyc": "^10.1.2",
        "raw-loader": "^0.5.1",
        "should": "^11.2.0",
        "style-loader": "^0.13.1",
        "webpack": "^2.2.1",
        "webpack-dev-server": "^2.4.1",
        "webpack-merge": "^3.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "33983b1f90d27ddab0e57d0dac403dce9bc7ecfd",
        "tarball": "https://registry.npmjs.org/sass-loader/-/sass-loader-6.0.3.tgz"
    },
    "engines": {
        "node": ">=4.0.0"
    },
    "files": [
        "lib",
        "README",
        "LICENSE"
    ],
    "gitHead": "54dc896dac6e81feb09f5f85334585b4418194c2",
    "homepage": "https://github.com/webpack-contrib/sass-loader#readme",
    "keywords": [
        "sass",
        "libsass",
        "webpack",
        "loader"
    ],
    "license": "MIT",
    "main": "lib/loader.js",
    "maintainers": [
        {
            "name": "jtangelder"
        },
        {
            "name": "akiran"
        },
        {
            "name": "peerigon"
        }
    ],
    "name": "sass-loader",
    "optionalDependencies": {},
    "peerDependencies": {
        "node-sass": "^4.0.0",
        "webpack": "^2.0.0"
    },
    "repository": {
        "type": "git",
        "url": "git://github.com/webpack-contrib/sass-loader.git"
    },
    "scripts": {
        "appveyor:test": "npm test",
        "create-spec": "node test/tools/runCreateSpec.js",
        "lint": "eslint lib test",
        "posttest": "npm run lint",
        "pretest": "npm run create-spec",
        "test": "nyc --all mocha -R spec -t 10000",
        "test-bootstrap-sass": "webpack-dev-server --config test/bootstrapSass/webpack.config.js --content-base ./test/bootstrapSass",
        "test-extract-text": "webpack --config test/extractText/webpack.config.js",
        "test-hmr": "webpack-dev-server --config test/hmr/webpack.config.js --content-base ./test/hmr --hot --inline",
        "test-source-map": "webpack-dev-server --config test/sourceMap/webpack.config.js --content-base ./test/sourceMap --inline",
        "test-watch": "webpack --config test/watch/webpack.config.js"
    },
    "version": "6.0.3",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
