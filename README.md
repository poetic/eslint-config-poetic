# Poetic Meteor Style

This package supplies an `eslint` configuration for working on Meteor apps.
It likes long walks on the beach, ES6 functionality (including modules!),
React components (now in JSX!), and most anything else needed to develop in
Meteor.

It uses [AirBnB's configuration](https://github.com/airbnb/javascript) as a
 base, and extends it with some Meteor-specific options.

## Installation
Run the following command to install the bits of `eslint` that we need:

`npm install -g eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react`

Then, add the `.eslintrc` and `.eslintignore` files to your app directory.

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

### Common Operations

As you develop in Meteor, you're going to be introducing globals:
Third party-packages, collection references, etc. `eslint` will complain that
these variables are undefined, which generally is a good thing; This keeps us
from attempting to access a variable that hasn't already been defined. With
globals, however, the variable has been defined elsewhere, and so we need to
tell `eslint` that it's cool to use them as such.

To do so, add a string representing the global to your project's `.eslintrc`'s
`global` object. Check out the file for some good examples of usage and syntax.
