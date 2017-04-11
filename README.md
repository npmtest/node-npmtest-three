# test coverage for  [three (v0.84.0)](http://threejs.org/)  [![npm package](https://img.shields.io/npm/v/npmtest-three.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-three) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-three.svg)](https://travis-ci.org/npmtest/node-npmtest-three)
#### JavaScript 3D library

[![NPM](https://nodei.co/npm/three.png?downloads=true)](https://www.npmjs.com/package/three)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-three/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-three/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-three/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-three/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-three/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-three/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-three/tree/gh-pages/build)|

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-three/build/screenCapture.buildCustomOrg.browser.coverage.html.png)](https://npmtest.github.io/node-npmtest-three/build/coverage.html/index.html)

[![test-report](https://npmtest.github.io/node-npmtest-three/build/screenCapture.buildCustomOrg.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmtest%252Fnode-npmtest-three%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-three/build/test-report.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-three/build/screenCapture.buildApidoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-three%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-three/build/apidoc.html)

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
        "eslint": "^3.10.1",
        "eslint-config-mdcs": "^4.2.2",
        "rollup": "^0.36.3",
        "rollup-watch": "^2.5.0",
        "uglify-js": "^2.6.0"
    },
    "directories": {
        "doc": "docs",
        "example": "examples",
        "test": "test"
    },
    "dist": {
        "shasum": "95be85a55a0fa002aa625ed559130957dcffd918",
        "tarball": "https://registry.npmjs.org/three/-/three-0.84.0.tgz"
    },
    "eslintConfig": {
        "extends": "mdcs"
    },
    "files": [
        "package.json",
        "LICENSE",
        "README.md",
        "build/three.js",
        "build/three.min.js",
        "build/three.module.js",
        "src",
        "examples/js",
        "examples/fonts"
    ],
    "gitHead": "3d8e0d43c6b79468a585cb37c63c3692a58125dc",
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
            "name": "bhouston",
            "email": "ben@exocortex.com"
        },
        {
            "name": "cabbibo",
            "email": "isaaclandoncohen@gmail.com"
        },
        {
            "name": "mrdoob",
            "email": "info@mrdoob.com"
        }
    ],
    "module": "build/three.module.js",
    "name": "three",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mrdoob/three.js.git"
    },
    "scripts": {
        "build": "rollup -c",
        "build-closure": "rollup -c && java -jar utils/build/compiler/closure-compiler-v20160713.jar --warning_level=VERBOSE --jscomp_off=globalThis --jscomp_off=checkTypes --externs utils/build/externs.js --language_in=ECMASCRIPT5_STRICT --js build/three.js --js_output_file build/three.min.js",
        "build-uglify": "rollup -c && uglifyjs build/three.js -cm --preamble \"// threejs.org/license\" > build/three.min.js",
        "dev": "rollup -c -w",
        "lint": "eslint src",
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "version": "0.84.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
