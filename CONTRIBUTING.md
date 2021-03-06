# Contributing #

## Important notes ##
Please don’t edit files in the `dist` subdirectory as they are generated via Gulp. You’ll find source code in the `src` subdirectory!

### Code style ###
Regarding code style like indentation and whitespace, **follow the conventions you see used in the source already.**

### PhantomJS ###
While Gulp can run the included unit tests via [PhantomJS](http://phantomjs.org/), this shouldn’t be considered a substitute for the real thing. Please be sure to test the `test/*.html` unit test file(s) in _actual_ browsers.

## Modifying the code ##
First, ensure that you have the latest [Node.js](http://nodejs.org/) and [npm](http://npmjs.org/) installed.

Test that Gulp and Bower are installed by running `gulp --version` and `bower --version`.  If the commands aren’t found, run `npm install -g gulp bower`.  For more information about installing the tools, see [gulpjs.com](http://gulpjs.com/) or [bower.io](http://bower.io/) respectively.

1. Fork and clone the repo.
2. Run `npm install` to install all build dependencies.
3. Run `bower install` to install the front-end dependencies.
4. Run `gulp` to build this project.

Assuming that you don’t see any errors, you’re ready to go. Just be sure to run `gulp` after making any changes, to ensure that nothing is broken.

## Submitting pull requests ##

1. Create a new branch, please don’t work in your `master` branch directly.
2. Add failing tests for the change you want to make. Run `gulp` to see the tests fail.
3. Fix stuff.
4. Run `gulp` to see if the tests pass. Repeat steps 2-4 until done.
5. Open `test/*.html` unit test file(s) in actual browser to ensure tests pass everywhere.
6. Update the documentation to reflect any changes.
7. Push to your fork and submit a pull request.
