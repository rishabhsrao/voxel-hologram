# voxel-hologram [:star:](http://voxel-hologram-rsr.herokuapp.com/dist)

> A minimal Hologram theme based on Voxel.

[![Travis](https://img.shields.io/travis/rishabhsrao/voxel-hologram.svg?style=flat-square "Build status")](https://travis-ci.org/rishabhsrao/voxel-hologram)
[![David](https://img.shields.io/david/rishabhsrao/voxel-hologram.svg?style=flat-square "Dependency status (Node modules)")](https://david-dm.org/rishabhsrao/voxel-hologram)
[![Gemnasium](https://img.shields.io/gemnasium/rishabhsrao/voxel-hologram.svg?style=flat-square "Dependency status (Ruby gems)")](https://gemnasium.com/rishabhsrao/voxel-hologram)
[![Code Climate](https://img.shields.io/codeclimate/github/rishabhsrao/voxel-hologram.svg?style=flat-square "Code Climate status")](https://codeclimate.com/github/rishabhsrao/voxel-hologram)
[![Coveralls](https://img.shields.io/coveralls/rishabhsrao/voxel-hologram.svg?style=flat-square "Test coverage status")](https://coveralls.io/r/rishabhsrao/voxel-hologram)
[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](license.md)


## :star: Live demo

See the [Voxel Hologram Example](https://github.com/rishabhsrao/voxel-hologram-example) project for a [live demo](http://voxel-hologram-example-rsr.herokuapp.com/dist/docs/index.html).


## :rowboat: Get started

This project depends on the following tools:

* [Node.js](http://nodejs.org)
* [Ruby](https://www.ruby-lang.org)
* [Bundler](http://bundler.io) gem

:tophat: **Tip** Use [nvm](https://github.com/creationix/nvm) and [rvm](http://rvm.io) for easy management of NodeJS and Ruby installations.

```
git clone git@github.com:rishabhsrao/voxel-hologram.git voxel-hologram
cd voxel-hologram
npm install
bundle install
./node_modules/.bin/bower install
./node_modules/.bin/gulp build && say awesome # Only on Mac OSX; use espeak on GNU/Linux. Windows users, sorry, no awesomeness for you!
```

:tophat: **Tip** If you have global installations of `bower` and `gulp`, then you can avoid typing the `./node_modules/.bin/` bit.

:tophat: **Tip** Downloading dependencies over `git://` may be blocked if you are behind a firewall. The solution is to configure Git to use `https://` instead of `git://`. Run the following to force Git to use HTTPS:

```
git config url.https://.insteadOf git://
# Undo using git config unset url.https://
```


## :nut_and_bolt: Build

This project is built using [Gulp](http://gulpjs.com).

You can run a task using `./node_modules/.bin/gulp {{task-name}}`. The following build tasks are available:

* **build** Creates a build artifact, ready for deployment.
* **clean:deploy** Cleans all generated artifacts, except the distribution artifact.
* **clean** Cleans the distribution artifact and any other generated artifacts.
* **image:minify** Compresses the image files using [gulp-imagemin](https://www.npmjs.com/package/gulp-imagemin).
* **script:lint** Lints the JavaScript files using [JSHint](https://github.com/jshint/jshint).
* **script:minify:json** Minifies the JSON files using [JSON Minify](https://www.npmjs.org/package/gulp-jsonminify).
* **script:minify** Minifies the JavaScript files using [UglifyJS](http://github.com/mishoo/UglifyJS).
* **script:optimize** Combines and optimizes all RequireJS modules into one file using [RequireJS Optimizer](http://requirejs.org/docs/optimization.html).
* **script:test:report** Uploads the code coverage report to [Coveralls](https://coveralls.io).
* **script:test:unit** Runs the JavaScript unit tests using [Karma](http://karma-runner.github.io) and [Jasmine](http://jasmine.github.io).
* **script:test** Runs all the JavaScript tests.
* **source** Copies the source files in the distribution artifact.
* **style:compile** Compiles the Sass files using [Compass](http://compass-style.org).
* **style:lint** Lints the Sass files using [SCSS-Lint](https://github.com/causes/scss-lint).

:tophat: **Tip** It's a good idea to occasionally run:

```
git gc
npm prune && npm install
bower prune && bower install
bundle clean --force && bundle install
```

... to keep your repository lean and mean.


## :scroll: License

See [license.md](license.md).
