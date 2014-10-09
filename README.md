squint
======

Squint is a verbose and pro-whitespace coding style. It favors specific naming conventions and generous whitespace. Code should be as self documenting as possible as well as easy on the eyes.

##Tools##
* **[scss-lint]()** - for enforcing Sass linting rules.
	* View scss-lint config file.
	* View documentation and reasoning behind this 	  config file.
* **[csscomb]()** - for convenience as well as some style options that scss-lint doesn't offer.
	* View css-comb config file.
* **[eslint]()** - for enforcing JavaScript linting rules.
	* View eslint config file.
* **[Gulp.js]()** - As streaming build system.

##Setup##

**Prerequisites**

* [node.js](http://nodejs.org/)
* [Ruby](https://www.ruby-lang.org/en/)
* [Gulp](https://github.com/gulpjs/gulp/)

1. Download all of the config files, and place them in your root directory.
2. Install scss-lint and respective Gulp plugin.
	* `gem install scss-lint`
	* `npm install --save-dev gulp-scss-lint`.
3. Install csscomb Gulp plugin.
	* `npm install gulp-csscomb --save-dev`
4. Install eslint Gulp plugin.
	* `npm install --save-dev gulp-eslint`
5. Add Gulp tasks for all 3 tools. See example gulpfile.js.