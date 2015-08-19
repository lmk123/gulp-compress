# gulp-compress

An easy-to-use module to compress your *.css , *.js and *.html files.

## Install

```
npm install gulp-compress
```

## Usage

```js
var gulp    = require('gulp'),
    options = {
       src: './src',
       dest: './dist'
    };

require('gulp-compress')(gulp, options);
```

There are few tasks added in your gulp:

 + `copy` : Copy files which are match [these glob](https://github.com/lmk123/gulp-compress/blob/master/index.js#L27) to `options.dest`
 + `compress-html`：Compress *.html files which are under `options.src` then output to `options.dest`
 + `compress-css`：Compress *.css files which are under `options.src` then output to `options.dest`
 + `compress-js`：Compress *.js files which are under `options.src` then output to `options.dest`
 + `compress`：It's run above tasks parallel.
 
 Now use them like this!

```
gulp compress
```

You may need [gulp-es6-sass](https://www.npmjs.com/package/gulp-es6-sass) else :)
 
## Options

All options and its default value are list on [here](https://github.com/lmk123/gulp-compress/blob/master/index.js#L8). It's really self-explanation.

## License
MIT
