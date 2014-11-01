
# JavaScript Coding Style


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

### Build Process

Projects should always have some form a build process to prepare for deployment. Use [Gulp](http://gulpjs.com) to create a `build` or `deploy` task that minifies and concatenates.

### Tests

Projects must include some form of unit or end to end testing.

- [Mocha](https://github.com/mochajs/mocha)
- [Karma](http://karma-runner.github.io/0.12/index.html)
- [Sinon](http://sinonjs.org/)
- [Chai](http://chaijs.com/)

### Beautiful, spacious syntax.

Use whitespace to improve readability. 

- Parens and braces should have spaces between them.
- Use Allman style indentation to clearly separate control statements from their code blocks. Additionally, it becomes easier to see dangling or mismatched braces.
- Groups of like items should be separated by 3 blank lines.

**Bad: cramped, hard to read syntax**

```
var isFast = (mileTime < 5) ? 'yes' : 'no';
```
```
for(var i=0;i<100;i++) someFunction();
```

**Good: generous whitespace**

```
var isFast;

if( mileTime < 5 )
{
	isFast = 'yes';
}
else
{
	isFast = 'no';
}
```
```
for( var i = 0; i < 100; i++ )
{
	someFunction(  );
}
```