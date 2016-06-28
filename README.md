# [![](http://squint-style.guide/images/squinty-face-small.svg)](http://squint-style.guide) squint-style 

Squint is a verbose and spacious coding style. It favors specific naming conventions and generous whitespace. Code should be as self documenting as possible and easy on the eyes.

-

> BE CONSISTENT.
 
> If you're editing code, take a few minutes to look at the code around you and determine its style. If they use spaces around all their arithmetic operators, you should too. If their comments have little boxes of hash marks around them, make your comments have little boxes of hash marks around them too.
 
> The point of having style guidelines is to have a common vocabulary of coding so people can concentrate on what you're saying rather than on how you're saying it. We present global style rules here so people know the vocabulary, but local style is also important. If code you add to a file looks drastically different from the existing code around it, it throws readers out of their rhythm when they go to read it. Avoid this." - [Google](https://google-styleguide.googlecode.com/svn/trunk/javascriptguide.xml)

-

> Code quality can be measured by how efficiently it can be changed.

-


This project aims to help developers in their pursuit of more efficiently writing code that is lasting and welcoming to change.

( ! ) Work in progress. Think this project could be better? Submit a pull request, issue, or [let me know](http://twitter.com/_rywar).

-

Read the **[Documentation](https://github.com/RyanWarner/squint-style/tree/master/docs)** to learn the defaults with code examples.

 Use the **[Config Files](https://github.com/RyanWarner/squint-style/tree/master/config-files)** in combination with the tools listed below to enforce good code style on your projects.


## Tools

A coding style guide is a complex thing. It can be hard to remember all the rules, especially when just starting out. In order to help enforce squint-style (or any style guide) you can use the following tools:

* **[scss-lint](https://github.com/causes/scss-lint)** - for enforcing Sass linting rules.
	* [View scss-lint config file](https://github.com/RyanWarner/squint-style/blob/master/config-files/scss-linting-config.yml).
	* [View documentation](https://github.com/RyanWarner/squint-style/blob/master/docs/scss-linting-documentation.md) and reasoning behind this config file.
* **[csscomb](http://csscomb.com/)** - for convenience as well as some style options that scss-lint doesn't offer.
	* [View css-comb config file](https://github.com/RyanWarner/squint-style/blob/master/config-files/.csscomb.json).
* **[eslint](http://eslint.org/)** - for enforcing JavaScript linting rules.
	* [View eslint config file](https://github.com/RyanWarner/squint-style/blob/master/config-files/.eslintrc).
	* [Shareable eslint config](https://www.npmjs.com/package/eslint-config-squint-style)
* **[Gulp.js](http://gulpjs.com/)** - As streaming build system.
	* [View example gulp file](https://github.com/RyanWarner/jade-sass-seed/blob/master/gulpfile.js).

## Setup

To setup the tools mentioned above in your project you can use these instructions as a guide. You can also use the example Gulp tasks as a starting point for your project.

**Prerequisites**

- [node.js](http://nodejs.org/)
- [Ruby](https://www.ruby-lang.org/en/)

1. Install [gulp.js](http://gulpjs.com/)
	- `npm install -g gulp`
2. Download all of the config files, and place them in your root directory.
	* `git clone https://github.com/RyanWarner/squint-style.git`
3. Install [scss-lint](https://github.com/causes/scss-lint) and respective Gulp plugin, [gulp-scss-lint](https://www.npmjs.org/package/gulp-scss-lint).
	* `gem install scss-lint`
	* `npm install --save-dev gulp-scss-lint`.
4. Install csscomb Gulp plugin, [gulp-csscomb](https://www.npmjs.org/package/gulp-csscomb).
	* `npm install gulp-csscomb --save-dev`
5. Install eslint Gulp plugin, [gulp-eslint](https://www.npmjs.org/package/gulp-eslint).
	* `npm install --save-dev gulp-eslint`
6. Add Gulp tasks for all 3 tools. See [example gulpfile.js](https://github.com/RyanWarner/jade-sass-seed/blob/master/gulpfile.js).


## Other CSS Style Guides

- [GitHub](https://github.com/styleguide/css)
- [Google](https://google-styleguide.googlecode.com/svn/trunk/htmlcssguide.xml)
- [Wordpress](https://make.wordpress.org/core/handbook/coding-standards/css/)
- [Idiomatic CSS](https://github.com/necolas/idiomatic-css)
- ["CSS Style Guides"](http://css-tricks.com/css-style-guides/) - CSS Tricks

## Other JavaScript Style Guides

- [Airbnb](https://github.com/airbnb/javascript)
- [Idiomatic JS](https://github.com/rwaldron/idiomatic.js)
- [Google](http://google-styleguide.googlecode.com/svn/trunk/javascriptguide.xml)
- [Dojo](http://dojotoolkit.org/community/styleGuide)
- [jQuery](http://contribute.jquery.org/style-guide/js/)

- - -
Inspired by [@lilhinx](http://twitter.com/lilhinx).
