# penguin.js-core

This package includes the build API for the penguin.js CMS.

## Usage

```js
'use strict'

const { build } = require('penguin.js-core')

// These are the options you can pass to the build command with their default
// values.
const templatePrefix = 'pack'
const databasePrefix = 'data'
const output = 'dist'

build({ templatePrefix, databasePrefix, output })
```

This will produce an output directory `dist/` that includes all statically
built files. The source for this directory is taken from the `pack/` directory.
Take a look at [penguin.js](https://github.com/domachine/penguin.js) to
understand how `pack/` is is produced.
