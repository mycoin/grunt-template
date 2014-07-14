# grunt-template-js

> Compiles HTML templates to JavaScript variables, jsonp and CMD.



## Getting Started
This plugin requires Grunt `~0.4.0`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-template-js --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-template-js');
```

*This plugin was designed to work with Grunt 0.4.x. If you're still using grunt v0.3.x it's strongly recommended that [you upgrade](http://gruntjs.com/upgrading-from-0.3-to-0.4).*



## `template` task
_Run this task with the `grunt template` command._

Task targets, files and options may be specified according to the grunt [Configuring tasks](http://gruntjs.com/configuring-tasks) guide.

### Options

#### mode
Type: `string`  
Default: `default`

available values are `compress`, `format` and `default`

#### wrap
Type: `Boolean`  
Default: false

Will transmit outputs to `CMD`.

### Usage Examples

There are three formats you can use to run this task.

#### Compiles HTML templates to JavaScript

```js
'template': {
    options: {
        mode: 'format',
        wrap: true
    },

    'build': {
        files: [{
            expand: true,
            cwd: 'src/html',
            src: '**/*.html',
            dest: 'src/html'
        }]
    }
}
```
---

Task submitted by [mycoin](https://github.com/mycoin/)

*This file was generated on Mon Jul 15 2013 20:45:46.*
