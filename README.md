# npmtest-in-view

#### basic test coverage for  [in-view (v0.6.1)](https://camwiegert.github.io/in-view)  [![npm package](https://img.shields.io/npm/v/npmtest-in-view.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-in-view) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-in-view.svg)](https://travis-ci.org/npmtest/node-npmtest-in-view)

#### Get notified when a DOM element enters or exits the viewport.

[![NPM](https://nodei.co/npm/in-view.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/in-view)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-in-view/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-in-view/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-in-view/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-in-view/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-in-view/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-in-view/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-in-view/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-in-view/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-in-view/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-in-view/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-in-view/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-in-view/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-in-view/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-in-view/build/test-report.html](https://npmtest.github.io/node-npmtest-in-view/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-in-view/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-in-view/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-in-view/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-in-view/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-in-view/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-in-view/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-in-view/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-in-view/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Cam Wiegert"
    },
    "ava": {
        "files": [
            "test/*js"
        ],
        "require": [
            "babel-register",
            "./test/helpers/setup-browser-env.js"
        ],
        "babel": "inherit"
    },
    "babel": {
        "plugins": [
            "lodash"
        ],
        "presets": [
            "es2015"
        ]
    },
    "bugs": {
        "url": "https://github.com/camwiegert/in-view/issues"
    },
    "dependencies": {
        "lodash": "^4.15.0"
    },
    "description": "Get notified when a DOM element enters or exits the viewport.",
    "devDependencies": {
        "ava": "^0.16.0",
        "babel-core": "^6.14.0",
        "babel-loader": "^6.2.5",
        "babel-plugin-lodash": "^3.2.8",
        "babel-preset-es2015": "^6.14.0",
        "babel-register": "^6.11.6",
        "eslint": "^3.3.1",
        "http-server": "^0.9.0",
        "jsdom": "^9.4.2",
        "lodash-webpack-plugin": "^0.10.0",
        "node-sass": "^3.8.0",
        "webpack": "^1.13.2"
    },
    "directories": {},
    "dist": {
        "shasum": "f9f99b5d5a6fe01359d9e19c570302a3121baf42",
        "tarball": "https://registry.npmjs.org/in-view/-/in-view-0.6.1.tgz"
    },
    "eslintConfig": {
        "extends": "eslint:recommended",
        "env": {
            "browser": true,
            "node": true
        },
        "parserOptions": {
            "ecmaVersion": 6,
            "sourceType": "module"
        }
    },
    "gitHead": "b6389d348df8b172c80f48ab554086333afcf03a",
    "homepage": "https://camwiegert.github.io/in-view",
    "license": "MIT",
    "main": "dist/in-view.min.js",
    "maintainers": [
        {
            "name": "camwiegert"
        }
    ],
    "name": "in-view",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/camwiegert/in-view.git"
    },
    "scripts": {
        "build": "NODE_ENV=production webpack -p",
        "docs": "npm run -s docs-server & npm run -s docs-js & npm run -s docs-css",
        "docs-css": "node-sass -w --output-style=compressed ./docs/lib/css/main.scss ./docs/lib/css/main.min.css",
        "docs-js": "NODE_ENV=production webpack -wp --config ./docs/docs.webpack.config.js",
        "docs-server": "http-server ./docs -o",
        "lint": "eslint src/**/*.js",
        "prepublish": "npm run -s test",
        "pretest": "npm run -s lint",
        "start": "NODE_ENV=production webpack -wp",
        "test": "ava -v"
    },
    "version": "0.6.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
