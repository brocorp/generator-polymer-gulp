
# Yeoman generator for Polymer projects using Gulp [![Build Status](https://secure.travis-ci.org/NicoArbogast/generator-polymer-gulp.png?branch=master)](https://travis-ci.org/NicoArbogast/generator-polymer-gulp)

![Yeoman + Polymer + Gulp](http://i.imgur.com/ZWA3ZSH.png "generator-polymer-gulp")

## Introduction

`generator-polymer-gulp` uses [Yeoman](http://yeoman.io) (the web's scaffolding tool for modern webapps) to set up a working environment for building [Polymer](http://www.polymer-project.org/) components, saving you time writing boilerplate.

This project was inspired by

- [generator-polymer](https://github.com/yeoman/generator-polymer)
- [Google Web Starter Kit](https://developers.google.com/web/starter-kit/)

## Features

This project uses

* [Gulp](http://gulpjs.com/) (the streaming build system) for automating your build cycle.
* [Browserify](http://browserify.org/) (js modules bundler) for building your js.
* [SASS](http://sass-lang.com/) (css with superpowers) for developing your css.
* [BrowserSync](http://www.browsersync.io/) (time-saving synchronised browser testing) for multi-browser/multi-device easy development with live reload.
* [Closure Compiler](https://developers.google.com/closure/compiler/) (js compiler) for packaging your js to download and run faster.
* [Vulcanize](https://github.com/Polymer/vulcanize) (build tool for HTMLImports and web components) for packaging your polymer components.

## Getting Started

Install:
```npm install -g generator-polymer-gulp```

Make a new dir && cd into it:
```mkdir my-polymer-component && cd $_```

Scaffold a new Polymer component:
```yo polymer-gulp```

Launch a dev web server watching dev files with live reload:
```gulp serve```

Build all assets for production and distribution:
```gulp build```

Clean / Rebuild everything:
```gulp```

## Folders structure

At bootstrap your working directory contains

* app/ : your application logic
* lib/ : external libs used (including .bower_components)

The build cycle will later create

* \_tmp/         : the app build for development (js browserifyd, css sassed)
* \_dist/        : the app built for production (js compiled, css uncssd, html minified)
* \_vulcanized/  : your polymer component built for distribution (csp, inline, raw)

## Options

* `--skip-install`

  Skips the automatic execution of `bower` and `npm` after scaffolding has finished.

## License

  Apache 2.0 License 2004
  Copyright (c) 2014 Nicolas Arbogast
