<div align="center">
  <img alt="Jekyll and Vue logos" src=".github/jekyll-vue.png" width="75%">
</div>

<h1 align="center">jekyll-vue-template</h1>

> A Jekyll project template that uses Vue.js single file components complete with webpack bundling and optimizations.

## Overview

jekyll-vue-template is an opinionated, but minimal boilerplate for creating statically generated sites with Jekyll and Vue.js. It supports Vue single file components and webpack optimizations including code-splitting and cache-control.

## Features

* Support for Vue single file components
* Vendor code-splitting with webpack 4
* Cache control for bundled assets using webpack 4
* Babel transpilation
* Sass language support in Vue single file components
* eslint with Vue style guide plugin
* Hot-reloading via BrowserSync

## Installation

The easiest way to use the jekyll-vue-template is to clone or fork this repo, then customize it to suit your needs.

### Install npm Packages

```console
$ npm i
```

### Install Ruby Gems

```console
$ bundle
```

## Usage

The `src` directory contains the Vue application and its components. Create single file components and mount them anywhere in your Jekyll pages, including layouts, markdown pages, or includes.

### Development

To run the jekyll-vue-template in a development environment, first compile assets with webpack:

```console
$ npm run dev
```

Alternatively you can use the `watch` command to watch for changes in your webpack-managed assets and automatically recompile.

```console
$ npm run watch
```

After assets have been built, spool up a development server with Jekyll:

```console
$ bundle exec jekyll s
```

### Production

To build for production, first compile webpack assets:

```console
$ npm run build
```

After assets have been built, generate the static files with Jekyll:

```console
$ bundle exec jekyll build
```

## Technical

jekyll-vue-template uses the following projects as critical workflow components:

* **Jekyll** `v3.8.5`
* **Vue** `v2.5.21`
* **webpack** `v4.28.3`

## License

MIT &copy; [Christopher Murphy](https://github.com/splode)

[Jekyll License Info](https://github.com/jekyll/jekyll/blob/master/LICENSE)

[Vue.js License Info](https://github.com/vuejs/vue/blob/master/LICENSE)
