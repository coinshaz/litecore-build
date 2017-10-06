# unitedcore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install unitedcore-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var unitedcoreTasks = require('unitedcore-build');

unitedcoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var unitedcoreTasks = require('unitedcore-build');
unitedcoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/coinshaz/unitedcore) on the main unitedcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/coinshaz/unitedcore/blob/master/LICENSE).

Copyright 2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
Copyright 2016 The Litecoin Core Developers
