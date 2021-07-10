# sass-exception

[![Release Version](https://img.shields.io/npm/v/sass-exception.svg)](https://www.npmjs.com/package/sass-exception)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

This Sass module provides functions to standardize exception messages.

## Install

### Requires

Install the package:

```bash
npm install sass-exception
```

Use the package like any other Sass module:

```scss
@use 'sass-exception';
```

Depending on your setup, you may need to configure `node_modules` as include path:

```js
const sass = require('sass');

sass.render({
  file: scss_filename,
  includePaths: ['node_modules']
});
```

## Public API

<dl>

  <dt><a href="//github.com/roydukkey/sass-module-exception/tree/master/src/exception/_is-separator-invalid.sass"><code>is-separator-invalid ( $value )</code></a></dt>
  <dd>Indicates whether a specified value is invalid for a separator parameter.</dd>

  <dt><a href="//github.com/roydukkey/sass-module-exception/tree/master/src/exception/_parameter.sass"><code>parameter ( $message, $context, $names... )</code></a></dt>
  <dd>Returns an error message stating an issue with one or more parameters.</dd>

  <dt><a href="//github.com/roydukkey/sass-module-exception/tree/master/src/exception/_parameter-type.sass"><code>parameter-type ( $context, $name, $value, $types... )</code></a></dt>
  <dd>Returns an error message stating a parameter received the wrong type.</dd>

  <dt><a href="//github.com/roydukkey/sass-module-exception/tree/master/src/exception/_separator.sass"><code>separator ( [$context] )</code></a></dt>
  <dd>Returns an error message stating a separator parameter or variable received the wrong value.</dd>

  <dt><a href="//github.com/roydukkey/sass-module-exception/tree/master/src/exception/_validate-index.sass"><code>validate-index ( $context, $name, $value, $iterable )</code></a></dt>
  <dd>Returns a valid index for the specified iterable; otherwise, an error message stating the reason the index is invalid.</dd>

  <dt><a href="//github.com/roydukkey/sass-module-exception/tree/master/src/exception/_variable.sass"><code>variable ( $message, $names... )</code></a></dt>
  <dd>Returns an error message stating an issue with one or more variables.</dd>

  <dt><a href="//github.com/roydukkey/sass-module-exception/tree/master/src/exception/_variable-type.sass"><code>variable-type ( $name, $value, $types... [, $message] )</code></a></dt>
  <dd>Returns an error message stating a variable received the wrong type.</dd>

</dl>

Don't see the function you're looking for? Request a [new feature](//github.com/roydukkey/sass-module-exception/issues/new) describing a use case.
