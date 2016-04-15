# Cartridge JavaScript [![Build Status](https://travis-ci.org/cartridge/cartridge-javascript.svg?branch=master)](https://travis-ci.org/cartridge/cartridge-javascript)

> JavaScript expansion pack for [Cartridge](https://github.com/cartridge/cartridge)

To use this module, you will need [cartridge-cli](https://github.com/cartridge/cartridge-cli) installed and have a cartridge project setup.

```sh
npm install cartridge-javascript --save-dev
```

This module adds the following to a project:

* JavaScript [concatination](https://github.com/contra/gulp-concat) and [minification](https://github.com/terinjokes/gulp-uglify)
* JavaScript [sourcemaps](https://github.com/floridoo/gulp-sourcemaps)
* JavaScript linting using [gulp-jshint](https://github.com/spalger/gulp-jshint)
* JavaScript documentation generation using [gulp-jsdoc3](https://github.com/mlucool/gulp-jsdoc3)

## Config

Once installed, the config file `task.scripts.js` is created and stored in the `_config` directory in the root of your cartridge project.

## Usage

This module provides the following gulp tasks

* `gulp scripts` - Task that runs all of the tasks mentioned below.
* `gulp scripts:bundle` - Concatinates all JS files into one file. When the `--prod` is provided the concatinated file is also minified. Sourcemaps are generated by default when no `--prod` flag is provided.
* `gulp scripts:lint` - Lints all JS files. Ignored if `--prod` is provided.
* `gulp scripts:docs` - Generates JS docs, for when [JSDocs](http://usejsdoc.org/) are used in source file.

* * * 

## Development
### Commit message standards [![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
Try and adhere as closely as possible to the [Angular commit messages guidelines](https://github.com/angular/angular.js/blob/master/CONTRIBUTING.md#-git-commit-guidelines).

[Commitizen](https://github.com/commitizen/cz-cli) is a command line tool which can help with this:
```sh
npm install -g commitizen
```
Now, simply use `git cz` instead of `git commit` when committing.
