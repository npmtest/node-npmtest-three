# npmtest-three

#### basic test coverage for  [three (v0.85.0)](http://threejs.org/)  [![npm package](https://img.shields.io/npm/v/npmtest-three.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-three) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-three.svg)](https://travis-ci.org/npmtest/node-npmtest-three)

#### JavaScript 3D library

[![NPM](https://nodei.co/npm/three.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/three)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-three/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-three/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-three/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-three/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-three/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-three/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-three/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-three/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-three/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-three/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-three/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-three/build/test-report.html](https://npmtest.github.io/node-npmtest-three/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-three/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-three/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-three/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-three/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-three/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-three/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-three/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-three/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "mrdoob"
    },
    "bugs": {
        "url": "https://github.com/mrdoob/three.js/issues"
    },
    "dependencies": {},
    "description": "JavaScript 3D library",
    "devDependencies": {
        "electron": "^1.6.1",
        "eslint": "^3.10.1",
        "eslint-config-mdcs": "^4.2.2",
        "qunitjs": "^2.1.1",
        "rollup": "^0.41.4",
        "rollup-watch": "^3.2.2",
        "uglify-js": "^2.6.0"
    },
    "directories": {
        "doc": "docs",
        "example": "examples",
        "test": "test"
    },
    "dist": {
        "shasum": "2efb33e8a449778fb8c71ac959e41bb81ef087d7",
        "tarball": "https://registry.npmjs.org/three/-/three-0.85.0.tgz"
    },
    "eslintConfig": {
        "extends": "mdcs"
    },
    "files": [
        "package.json",
        "bower.json",
        "LICENSE",
        "README.md",
        "build/three.js",
        "build/three.min.js",
        "build/three.module.js",
        "src",
        "examples/js",
        "examples/fonts"
    ],
    "gitHead": "f5b9e5a3b3305677271b0f5a0b77d1723fdef967",
    "homepage": "http://threejs.org/",
    "jsnext:main": "build/three.module.js",
    "keywords": [
        "three",
        "three.js",
        "3d",
        "webgl"
    ],
    "license": "MIT",
    "main": "build/three.js",
    "maintainers": [
        {
            "name": "bhouston"
        },
        {
            "name": "cabbibo"
        },
        {
            "name": "mrdoob"
        }
    ],
    "module": "build/three.module.js",
    "name": "three",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mrdoob/three.js.git"
    },
    "scripts": {
        "build": "rollup -c",
        "build-closure": "rollup -c && java -jar utils/build/compiler/closure-compiler-v20160713.jar --warning_level=VERBOSE --jscomp_off=globalThis --jscomp_off=checkTypes --externs utils/build/externs.js --language_in=ECMASCRIPT5_STRICT --js build/three.js --js_output_file build/three.min.js",
        "build-test": "rollup -c test/rollup.unit.config.js",
        "build-uglify": "rollup -c && uglifyjs build/three.js -cm --preamble \"// threejs.org/license\" > build/three.min.js",
        "dev": "rollup -c -w -m inline",
        "editor": "electron ./editor/main.js",
        "lint": "eslint src",
        "test": "rollup -c test/rollup.unit.config.js -w"
    },
    "version": "0.85.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
