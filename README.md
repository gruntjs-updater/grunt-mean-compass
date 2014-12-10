# grunt-mean-compass

> Compile mean.io sass-compass files.

## Getting Started
This plugin requires Grunt `~0.4.5`, Grant-contrib-compass `~1.0.1`, and using [Mean.io](http://www.mean.io)

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-mean-compass --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-mean-compass');
```

## The "meanCompass" task

### Overview
In your project's Gruntfile, add a section named `meanCompass` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  meanCompass: {
    options: {
      // Task-specific compass options go here. 
    },
    src: [] //glob files
  },
});
```

### Options

See options as described in [Grunt Compass](https://github.com/gruntjs/grunt-contrib-compass#options)

### Usage Examples

#### Default Options
In this example, the default options are used to do something with whatever. So if the `testing` file has the content `Testing` and the `123` file had the content `1 2 3`, the generated result would be `Testing, 1 2 3.`

```js
grunt.initConfig({
  mean_compass: {
    options: {},
    files: ['!bower_components/**', '!packages/contrib/**', 'packages/**/public/**/*.scss'],
  },
});
```

#### Custom Options
In this example, custom options are used to do something else with whatever else. So if the `testing` file has the content `Testing` and the `123` file had the content `1 2 3`, the generated result in this case would be `Testing: 1 2 3 !!!`

```js
grunt.initConfig({
  mean_compass: {
    options: {
      sourcemap: true
    },
    files: ['!bower_components/**', '!packages/contrib/**', 'packages/**/public/**/*.scss'],
  },
});
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
_(Nothing yet)_
