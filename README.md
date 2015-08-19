# gulp-es6-sass

用于精简 *.css、*.js 与 *.html 文件的模块。

## 安装与使用

通过 npm 安装：

```
npm install gulp-compress
```

然后在代码里使用：

```js
var gulp    = require('gulp'),
    options = {
       src: './src',
       dest: './dist'
    };

require('gulp-compress')(gulp, options);
```

这样就有五个任务添加到了你的 gulp 中：

 + `copy` : 将 `options.src` 下的[这些文件](https://github.com/lmk123/gulp-compress/blob/master/index.js#L27)复制到 `options.dest` 中
 + `compress-html`：将 `options.src` 下的所有 `html` 文件精简并输出到 `options.dest` 中
 + `compress-css`：将 `options.src` 下的所有 `css` 文件精简并输出到 `options.dest` 中
 + `compress-js`：将 `options.src` 下的所有 `js` 文件精简并输出到 `options.dest` 中
 + `compress`：并行执行上面四个任务
 
## 设置项
 
 所有设置项及其默认值都在[这里](https://github.com/lmk123/gulp-compress/blob/master/index.js#L8)。

## 许可
MIT
