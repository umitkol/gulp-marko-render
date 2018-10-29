# gulp-rev 

A Gulp plugin for Marko template engine.

## Install

```
$ npm install --save-dev gulp-marko-render
```


## Usage

```js
const gulp = require('gulp');
const markoRender = require('gulp-marko-render');

gulp.task('default', () =>
	gulp.src('src/*.marko')
		.pipe(markoRender())
		.pipe(gulp.dest('dist'))
);
```

## With Marko Options

```js
const gulp = require('gulp');
const markoRender = require('gulp-marko-render');

gulp.task('default', () =>
	gulp.src('src/*.marko')
		.pipe(markoRender({
			writeToDisk: false,
			preserveWhitespace: true,
			ext: "html"
		}))
		.pipe(gulp.dest('dist'))
);
```
