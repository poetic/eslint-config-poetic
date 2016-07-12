# Poetic Meteor Style

[![travis][travis-image]][travis-url]
[![npm][npm-image]][npm-url]
[![semantic-release][semantic-release-image]][semantic-release-url]

[travis-image]:            https://img.shields.io/travis/poetic/eslint-config-poetic.svg?branch=master
[travis-url]:              https://travis-ci.org/poetic/eslint-config-poetic
[npm-image]:               https://img.shields.io/npm/v/eslint-config-poetic.svg
[npm-url]:                 https://npmjs.org/package/eslint-config-poetic
[semantic-release-image]:  https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg
[semantic-release-url]:    https://github.com/semantic-release/semantic-release

This linter package is based on [AirBnB's configuration](https://github.com/airbnb/javascript).

## Installation

1. `npm install --save-dev eslint-config-poetic`
2. add `"extends": "poetic"` to your .eslintrc

## Usage
To run `eslint` from the command line, try this from your app root directory:

`eslint --ext .js,.jsx .`

### Vim Integration
Install the Syntastic plugin, then add the following to your .vimrc:

```
let g:syntastic_javascript_checkers=['eslint']
let g:syntastic_javascript_eslint_args="--ext .js,.jsx"
```

*Be sure to remove any other lines that set `syntastic_javascript_checkers`,
 if they exist.*
