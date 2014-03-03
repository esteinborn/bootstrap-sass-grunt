# Bootstrap SASS for Grunt

The original version of [bootstrap-sass](https://github.com/twbs/bootstrap-sass) was built for Ruby users, and confused the crap out of me. I ported it to use a Grunt build process. I will also update when [libsass support gets fixed](https://github.com/twbs/bootstrap-sass/issues/494).

This should hopefully be a drop and replace for new versions of boostrap-sass.

It pulls in [bootstrap-sass](https://github.com/twbs/bootstrap-sass) as a submodule.

### Start here if you are using git command line:

You must run two commands:
`git submodule init` to initialize your local configuration file

`git submodule update` to fetch all the data from that project and check out the appropriate commit.

### Start here if you are using a GUI client:

Run `npm install` to install all dependencies.

Run `grunt scaffold-bootstrap` to scaffold all the files for Bootstrap-SASS-Grunt.

## Bootstrap for Sass


[![Build Status](https://secure.travis-ci.org/twbs/bootstrap-sass.png?branch=master)](http://travis-ci.org/twbs/bootstrap-sass)

`bootstrap-sass` is a Sass-powered version of [Bootstrap](http://github.com/twbs/bootstrap), ready to drop right into your Sass powered applications.

## Compiling CSS and JavaScript

Bootstrap uses [Grunt](http://gruntjs.com/) with convenient methods for working with the framework. It's how we compile our code, run tests, and more. To use it, install the required dependencies as directed and then run some Grunt commands.

### Install Grunt

From the command line:

1. Install `grunt-cli` globally with `npm install -g grunt-cli`.
2. Navigate to the root `/bootstrap` directory, then run `npm install`. npm will look at [package.json](https://github.com/twbs/bootstrap/blob/master/package.json) and automatically install the necessary local dependencies listed there.

When completed, you'll be able to run the various Grunt commands provided from the command line.

**Unfamiliar with `npm`? Don't have node installed?** That's a-okay. npm stands for [node packaged modules](http://npmjs.org/) and is a way to manage development dependencies through node.js. [Download and install node.js](http://nodejs.org/download/) before proceeding.

### Available Grunt commands

#### Build Development code - `grunt`
Run `grunt` to run tests locally and compile the CSS and JavaScript into `/dist`. **Uses [SASS](http://sass-lang.com/) and [JSHint](http://www.jshint.com/).**

#### Build Production code - `grunt dist`
`grunt dist` creates the `/dist` directory with compiled files. **Uses [SASS](http://sass-lang.com/) and [UglifyJS](http://lisperator.net/uglifyjs/).**

#### Watch - `grunt watch`
This is a convenience method for watching SASS & JavaScript files and automatically building them whenever you save.

### Troubleshooting dependencies

Should you encounter problems with installing dependencies or running Grunt commands, uninstall all previous dependency versions (global and local). Then, re-run `npm install`.

