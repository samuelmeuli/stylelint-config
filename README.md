# stylelint-config

This is my personal configuration for [Stylelint](https://github.com/stylelint/stylelint). It includes rules for CSS and SCSS and enforces a reasonable property order.

## Overview

The rules are based on the [sass-guidelines](https://github.com/bjankord/stylelint-config-sass-guidelines) and [rational-order](https://github.com/constverum/stylelint-config-rational-order) configurations and include a couple of custom additions and deletions.

The configuration is compatible with [Prettier](https://github.com/prettier/prettier) (if it's configured to use tabs for indentation).

## Usage

1. Install the required packages:

```sh
yarn add --dev stylelint @samuelmeuli/stylelint-config
```

2. Add a Stylelint configuration to your `package.json` file:

```js
{
  // ...
  "stylelint": {
    "extends": "@samuelmeuli/stylelint-config"
  }
}
```

3. Add the linting script(s) you need to your `package.json` file:

```json
{
  "scripts": {
    "lint:css": "stylelint --fix --max-warnings 0 src/**/*.css",
    "lint:scss": "stylelint --fix --max-warnings 0 --syntax scss src/**/*.scss"
  }
}
```
