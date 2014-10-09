
##SCSS Coding Style##

###Spacing and Indentation###

* Properties and values should be clearly separated from their selectors using Allman Style indentation, meaning a new line before `{`.

* To increase readability, put spaces between parenthesis `(  )`.

* Additionally, there should be a space after every `,` and a space after every `:`.

* There should always be a new line at the end of every file.

###Formatting###

* Use lowercase letters in hex codes.
* Use `//` for comments, not `/* */`.
* Always specify leading 0s, like `0.5`.
* Use longhand values, be explicit and avoid shorthand.
* Selectors be written in hyphenated lowercase, not [CamelCase](http://en.wikipedia.org/wiki/CamelCase) or [snake_case](http://en.wikipedia.org/wiki/Snake_case).

###Good Practice###

* Limit use of IDs, and never add unnecessary selectors. Some people even think you [shouldn't use ID selectors at all.](http://screwlewse.com/2010/07/dont-use-id-selectors-in-css/)
* Avoid unecessary nesting. If your CSS looks like your HTML, something is wrong. Limit nesting to 3 levels deep.

###File Structure###

###Starting Point###

Use [sass-seed](https://github.com/RyanWarner/sass-seed) as a base for your projects.