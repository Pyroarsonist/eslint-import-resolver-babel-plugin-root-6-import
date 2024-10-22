# eslint-import-resolver-babel-plugin-root-import

## ⚠️ babel-plugin-root-import peer dependency bumped to 6.6.0 ⚠️

A [babel-plugin-root-import] resolver for [eslint-plugin-import].

This is a fork of [eslint-import-resolver-babel-root-import] that works with 
latest version of babel plugin.

## Installation

```sh
npm install --save-dev eslint-plugin-import eslint-import-resolver-babel-plugin-root-import
```

## Usage

Inside your `.eslintrc` file, pass this resolver to `eslint-plugin-import`:

```json
"settings": {
  "import/resolver": "babel-plugin-root-import"
}
```

And see [babel-plugin-root-import] to know how to configure your prefix/suffix. 
Configuration will be parsed down from `.babelrc` file

### Example

```json
{
  "extends": "airbnb",
  "rules": {},
  "settings": {
    "import/resolver": {
      "babel-plugin-root-import": {}
    }
  }
}
```

Or if you don't use `.babelrc` and keep your babel configuration in, say, webpack
config you can pass those options to resolver directly through `.eslintrc` file:

```json
{
  "extends": "airbnb",
  "rules": {},
  "settings": {
    "import/resolver": {
      "babel-plugin-root-import": {
        "rootPathPrefix": "@",
        "rootPathSuffix": "src/js"
      }
    }
  }
}
```

## License

MIT, see [LICENSE.md](/LICENSE.md) for details.


[babel-plugin-root-import]: https://github.com/entwicklerstube/babel-plugin-root-import
[eslint-plugin-import]: https://github.com/benmosher/eslint-plugin-import
[eslint-import-resolver-babel-root-import]: https://github.com/olalonde/eslint-import-resolver-babel-root-import
