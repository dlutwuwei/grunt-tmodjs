# grunt-tmodjs
[![NPM](https://nodei.co/npm/grunt-tmodjs.png)](https://nodei.co/npm/grunt-tmodjs/)

> grunt plugins for latest tmodjs

## Getting Started
This plugin requires Grunt `~0.4.5`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-tmodjs --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-tmodjs');
```

## The "tmod" task

### Overview
In your project's Gruntfile, add a section named `tmod` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  tmod: {
    options: {
      // the same as tmodjs
    },
    files: {
      src: 'tpl/'// Target-specific file lists and/or options go here.
    },
  },
});
```

### Options

#### options.separator
Type: `String`
Default value: `',  '`

A string value that is used to do something with whatever.

#### options.punctuation
Type: `String`
Default value: `'.'`

A string value that is used to do something else with whatever else.

### Usage Examples

#### Default Options
In this example, the default options are used to do something with whatever. So if the `testing` file has the content `Testing` and the `123` file had the content `1 2 3`, the generated result would be `Testing, 1 2 3.`

```js
grunt.initConfig({
  tmod: {
    options: {
        output: "js/",
        charset: "utf-8",
        syntax: "native",
        type: "templatejs",
        runtime:"template.js",
        combo: true,
        minify: true
    },
    files: {
      'src': 'tpl/',
    },
  },
});
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
_(Nothing yet)_
