# grunt-sass-recursive-import

> Recursively includes SASS Partials in all Subdirectories

## Getting Started
This plugin requires Grunt `~0.4.5`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-sass-recursive-import --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-sass-recursive-import');
```

## The "sass_recursive_import" task

### Overview
Find any SASS partial (beginning with an underscore `_`) which resides inside the directory of `main.scss` and its sub-directories and import them into `main.scss`.

```js
grunt.initConfig({
  sass_recursive_import: {
    options: {},
    files: {
      dest: ['src/scss/main.scss']
    },
  },
});
```
