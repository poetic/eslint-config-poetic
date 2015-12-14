#Poetic Meteor Style

This package supplies an `eslint` configuration for working on Meteor apps.
It likes long walks on the beach, ES6 functionality (including modules!), 
React components (now in JSX!), and most anything else under the sun.

It uses [AirBnB's configuration](https://github.com/airbnb/javascript) as a
 base, and extends it with some Meteor-specific options.

## Installation
Run the following command to install the bits of `eslint` that we need:

`npm install --save-dev eslint-config-airbnb eslint-plugin-react eslint`

If you would like to use `eslint` in `vim`, add the following line to your
`.vimrc`:

`let g:syntastic_javascript_checkers=['eslint']`

*Be sure to remove any other lines that set `syntastic_javascript_checkers`,
 if they exist.*

## Usage
Add the `.eslintrc` in this repo to your app directory. To run `eslint` from
the command line, try `eslint .` from your app directory.
