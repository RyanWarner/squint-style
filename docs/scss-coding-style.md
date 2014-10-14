
## SCSS Coding Style

### Spacing and Indentation

* Properties and values should be clearly separated from their selectors using Allman Style indentation, meaning a new line before `{`.
* To increase readability, put spaces between parenthesis `(  )`.
* Additionally, there should be a space after every `,` and a space after every `:`.
* Use `tabs` for semantic indentation, and `spaces` for presentational spacing.
* There should always be a new line at the end of every file.

### Formatting

* Use lowercase letters in hex codes.
* Use `'` not `"`.
* Use `//` for comments, not `/* */`.
* Always specify leading 0s, like `0.5`.
* Use longhand values, be explicit and avoid shorthand.
* Selectors be written in hyphenated lowercase, not [CamelCase](http://en.wikipedia.org/wiki/CamelCase) or [snake_case](http://en.wikipedia.org/wiki/Snake_case).

### Good Practice

* Limit use of IDs, and never add unnecessary selectors. Some people even think you [shouldn't use ID selectors at all.](http://screwlewse.com/2010/07/dont-use-id-selectors-in-css/)
* Avoid unecessary nesting. If your CSS looks like your HTML, something is wrong. Limit nesting to 3 levels deep. See SMACSS on [depth of applicability](http://smacss.com/book/applicability).

### File Structure

```
scss
├── main.scss
└── partials
    ├── base.scss
    ├── breakpoints.scss
    ├── reset.scss
    ├── mixins.scss
    ├── variables.scss
    └── module-directory
    	 └── component.scss
```

`main.scss` is used only for importing all other files, sort of like a table of contents. Nothing here except for `@import`.
A `module-directory` is a place to put styles for a module or component, such as all the styles for one page, or all the styles for a toggle switch. Any sizable website or application will have mutliple component folders, named after what they are.

### Starting Point

Use [sass-seed](https://github.com/RyanWarner/sass-seed) as a base for your projects.