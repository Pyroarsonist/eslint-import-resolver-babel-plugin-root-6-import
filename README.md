# eslint-import-resolver-babel-root-import

A [babel-plugin-root-import] resolver for [eslint-plugin-import].

:warning: This is a fork of [eslint-import-resolver-babel-root-import] that works with 
latest version of babel plugin. It will either go away if changes are merged or will be 
published to npm, because [other fork][eslint-import-resolver-babel-plugin-root-import]
doesn't do a good job. 

## Installation

```sh
npm install --save-dev eslint-plugin-import eslint-import-resolver-babel-root-import
```

## Usage

Inside your `.eslintrc` file, pass this resolver to `eslint-plugin-import`:
```
"settings": {
  "import/resolver": "@unconfident/eslint-import-resolver-babel-plugin-root-import"
}
```

And see [babel-plugin-root-import] to know how to configure
your prefix/suffix.

### Example

```json
{
  "extends": "airbnb",
  "rules": {},
  "settings": {
    "import/resolver": {
      "@unconfident/eslint-import-resolver-babel-plugin-root-import": {}
    }
  }
}
```

## License

MIT, see [LICENSE.md](/LICENSE.md) for details.


[babel-plugin-root-import]: https://github.com/entwicklerstube/babel-plugin-root-import
[eslint-plugin-import]: https://github.com/benmosher/eslint-plugin-import
[eslint-import-resolver-babel-root-import]: https://github.com/olalonde/eslint-import-resolver-babel-root-import
[eslint-import-resolver-babel-plugin-root-import]: https://github.com/bingqichen/eslint-import-resolver-babel-plugin-root-import
