squint
======

( ! ) Work in progress. Think this project could be better? [Let me know](http://twitter.com/_rywar).

Squint is a verbose and spacious coding style. It favors specific naming conventions and generous whitespace. Code should be as self documenting as possible as well as easy on the eyes.

### [Config Files]()
### [Documentation]()

## Tools
* **[scss-lint]()** - for enforcing Sass linting rules.
	* [View scss-lint config file](https://github.com/RyanWarner/squint-style/blob/master/config-files/scss-linting-config.yml).
	* [View documentation](https://github.com/RyanWarner/squint-style/blob/master/docs/scss-linting-documentation.md) and reasoning behind this config file.
* **[csscomb]()** - for convenience as well as some style options that scss-lint doesn't offer.
	* [View css-comb config file](https://github.com/RyanWarner/squint-style/blob/master/config-files/.csscomb.json).
* **[eslint]()** - for enforcing JavaScript linting rules.
	* [View eslint config file]().
* **[Gulp.js]()** - As streaming build system.
	* [View example gulp file]().

## Setup

**Prerequisites**

- [node.js](http://nodejs.org/)
- [Ruby](https://www.ruby-lang.org/en/)
- [Gulp](https://github.com/gulpjs/gulp/)

1. Download all of the config files, and place them in your root directory.
	* `git clone https://github.com/RyanWarner/squint.git`
2. Install scss-lint and respective Gulp plugin.
	* `gem install scss-lint`
	* `npm install --save-dev gulp-scss-lint`.
3. Install csscomb Gulp plugin.
	* `npm install gulp-csscomb --save-dev`
4. Install eslint Gulp plugin.
	* `npm install --save-dev gulp-eslint`
5. Add Gulp tasks for all 3 tools. See example gulpfile.js.

- - -

"BE CONSISTENT.

If you're editing code, take a few minutes to look at the code around you and determine its style. If they use spaces around all their arithmetic operators, you should too. If their comments have little boxes of hash marks around them, make your comments have little boxes of hash marks around them too.

The point of having style guidelines is to have a common vocabulary of coding so people can concentrate on what you're saying rather than on how you're saying it. We present global style rules here so people know the vocabulary, but local style is also important. If code you add to a file looks drastically different from the existing code around it, it throws readers out of their rhythm when they go to read it. Avoid this." - [Google](https://google-styleguide.googlecode.com/svn/trunk/javascriptguide.xml)

- - -
Inspired by [@lilhinx](htt{:://twitter.com/lilhinx).