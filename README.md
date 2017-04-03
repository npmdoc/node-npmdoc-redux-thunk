# api documentation for  [redux-thunk (v2.2.0)](https://github.com/gaearon/redux-thunk)  [![npm package](https://img.shields.io/npm/v/npmdoc-redux-thunk.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-redux-thunk) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-redux-thunk.svg)](https://travis-ci.org/npmdoc/node-npmdoc-redux-thunk)
#### Thunk middleware for Redux.

[![NPM](https://nodei.co/npm/redux-thunk.png?downloads=true)](https://www.npmjs.com/package/redux-thunk)

[![apidoc](https://npmdoc.github.io/node-npmdoc-redux-thunk/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-redux-thunk_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-redux-thunk/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-redux-thunk/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-redux-thunk/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Dan Abramov",
        "email": "dan.abramov@me.com"
    },
    "bugs": {
        "url": "https://github.com/gaearon/redux-thunk/issues"
    },
    "dependencies": {},
    "description": "Thunk middleware for Redux.",
    "devDependencies": {
        "babel-cli": "^6.6.5",
        "babel-core": "^6.6.5",
        "babel-eslint": "^5.0.0-beta4",
        "babel-loader": "^6.2.4",
        "babel-plugin-check-es2015-constants": "^6.6.5",
        "babel-plugin-transform-es2015-arrow-functions": "^6.5.2",
        "babel-plugin-transform-es2015-block-scoped-functions": "^6.6.5",
        "babel-plugin-transform-es2015-block-scoping": "^6.6.5",
        "babel-plugin-transform-es2015-classes": "^6.6.5",
        "babel-plugin-transform-es2015-computed-properties": "^6.6.5",
        "babel-plugin-transform-es2015-destructuring": "^6.6.5",
        "babel-plugin-transform-es2015-for-of": "^6.6.0",
        "babel-plugin-transform-es2015-function-name": "^6.5.0",
        "babel-plugin-transform-es2015-literals": "^6.5.0",
        "babel-plugin-transform-es2015-modules-commonjs": "^6.6.5",
        "babel-plugin-transform-es2015-object-super": "^6.6.5",
        "babel-plugin-transform-es2015-parameters": "^6.6.5",
        "babel-plugin-transform-es2015-shorthand-properties": "^6.5.0",
        "babel-plugin-transform-es2015-spread": "^6.6.5",
        "babel-plugin-transform-es2015-sticky-regex": "^6.5.0",
        "babel-plugin-transform-es2015-template-literals": "^6.6.5",
        "babel-plugin-transform-es2015-unicode-regex": "^6.5.0",
        "babel-plugin-transform-es3-member-expression-literals": "^6.5.0",
        "babel-plugin-transform-es3-property-literals": "^6.5.0",
        "chai": "^3.2.0",
        "cross-env": "^1.0.7",
        "eslint": "^1.10.2",
        "eslint-config-airbnb": "1.0.2",
        "eslint-plugin-react": "^4.1.0",
        "mocha": "^2.2.5",
        "redux": "^3.4.0",
        "rimraf": "^2.5.2",
        "typescript": "^1.8.10",
        "typescript-definition-tester": "0.0.4",
        "webpack": "^1.12.14"
    },
    "directories": {},
    "dist": {
        "shasum": "e615a16e16b47a19a515766133d1e3e99b7852e5",
        "tarball": "https://registry.npmjs.org/redux-thunk/-/redux-thunk-2.2.0.tgz"
    },
    "files": [
        "lib",
        "es",
        "src",
        "dist",
        "index.d.ts"
    ],
    "gitHead": "4f96ec0239453623adde857b7e7ad8c4f2897bf1",
    "homepage": "https://github.com/gaearon/redux-thunk",
    "jsnext:main": "es/index.js",
    "keywords": [
        "redux",
        "thunk",
        "middleware",
        "redux-middleware",
        "flux"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "aikoven",
            "email": "dan.lytkin@gmail.com"
        },
        {
            "name": "gaearon",
            "email": "dan.abramov@gmail.com"
        },
        {
            "name": "timdorr",
            "email": "timdorr@timdorr.com"
        }
    ],
    "name": "redux-thunk",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/gaearon/redux-thunk.git"
    },
    "scripts": {
        "build": "npm run build:commonjs && npm run build:umd && npm run build:umd:min && npm run build:es",
        "build:commonjs": "cross-env BABEL_ENV=commonjs babel src --out-dir lib",
        "build:es": "cross-env BABEL_ENV=es babel src --out-dir es",
        "build:umd": "cross-env BABEL_ENV=commonjs NODE_ENV=development webpack",
        "build:umd:min": "cross-env BABEL_ENV=commonjs NODE_ENV=production webpack",
        "clean": "rimraf lib dist es",
        "lint": "eslint src test",
        "posttest": "npm run lint",
        "prepublish": "npm run clean && npm run test && npm run build",
        "test": "cross-env BABEL_ENV=commonjs mocha --compilers js:babel-core/register --reporter spec test/*.js"
    },
    "typings": "./index.d.ts",
    "version": "2.2.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module redux-thunk](#apidoc.module.redux-thunk)
1.  boolean <span class="apidocSignatureSpan">redux-thunk.</span>__esModule
1.  [function <span class="apidocSignatureSpan">redux-thunk.</span>default (_ref)](#apidoc.element.redux-thunk.default)

#### [module redux-thunk.default](#apidoc.module.redux-thunk.default)
1.  [function <span class="apidocSignatureSpan">redux-thunk.</span>default (_ref)](#apidoc.element.redux-thunk.default.default)
1.  [function <span class="apidocSignatureSpan">redux-thunk.default.</span>withExtraArgument (extraArgument)](#apidoc.element.redux-thunk.default.withExtraArgument)



# <a name="apidoc.module.redux-thunk"></a>[module redux-thunk](#apidoc.module.redux-thunk)

#### <a name="apidoc.element.redux-thunk.default"></a>[function <span class="apidocSignatureSpan">redux-thunk.</span>default (_ref)](#apidoc.element.redux-thunk.default)
- description and source-code
```javascript
default = function (_ref) {
  var dispatch = _ref.dispatch,
      getState = _ref.getState;
  return function (next) {
    return function (action) {
      if (typeof action === 'function') {
        return action(dispatch, getState, extraArgument);
      }

      return next(action);
    };
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.redux-thunk.default"></a>[module redux-thunk.default](#apidoc.module.redux-thunk.default)

#### <a name="apidoc.element.redux-thunk.default.default"></a>[function <span class="apidocSignatureSpan">redux-thunk.</span>default (_ref)](#apidoc.element.redux-thunk.default.default)
- description and source-code
```javascript
default = function (_ref) {
  var dispatch = _ref.dispatch,
      getState = _ref.getState;
  return function (next) {
    return function (action) {
      if (typeof action === 'function') {
        return action(dispatch, getState, extraArgument);
      }

      return next(action);
    };
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.redux-thunk.default.withExtraArgument"></a>[function <span class="apidocSignatureSpan">redux-thunk.default.</span>withExtraArgument (extraArgument)](#apidoc.element.redux-thunk.default.withExtraArgument)
- description and source-code
```javascript
function createThunkMiddleware(extraArgument) {
  return function (_ref) {
    var dispatch = _ref.dispatch,
        getState = _ref.getState;
    return function (next) {
      return function (action) {
        if (typeof action === 'function') {
          return action(dispatch, getState, extraArgument);
        }

        return next(action);
      };
    };
  };
}
```
- example usage
```shell
...
## Injecting a Custom Argument

Since 2.1.0, Redux Thunk supports injecting a custom argument using the 'withExtraArgument' function:

'''js
const store = createStore(
reducer,
applyMiddleware(thunk.withExtraArgument(api))
)

// later
function fetchUser(id) {
return (dispatch, getState, api) => {
  // you can use api here
}
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
