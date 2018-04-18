# gulp-dot-precompiler-es6
This plugin is built on top of [gulp-dot-precompiler](https://github.com/kentliau/gulp-dot-precompiler) with support for ES6 syntax



```
let gulp = require('gulp');
let dot  = require('gulp-dot-precompiler-es6');
let ext_replace = require('gulp-ext-replace');


gulp.task('dot', function () {
    return gulp.src(['./src/main/js/templates/**/*.html'])
        .pipe(dot()).pipe(ext_replace('.js'))
        .pipe(gulp.dest('./src/main/js/compiled-templates'));
});
```
