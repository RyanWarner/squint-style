
# JavaScript Coding Style

This is a living documentation detailing the squint-style JavaScript best practices.

## Spacing and Indentation

- Properties and values should be clearly separated from their selectors using Allman Style indentation, meaning a new line before `{`.
- To increase readability, put spaces between parenthesis `(  )`.
	- See [space-in-parens](https://github.com/RyanWarner/squint-style/blob/master/docs/javascript-linting-documentatio.md#space-in-parens) and [new-parens](https://github.com/RyanWarner/squint-style/blob/master/docs/javascript-linting-documentatio.md#new-parens) linters.
- Additionally, there should be a space after every `,` and a space after every `:`.
- Use `tabs` for semantic indentation, and `spaces` for presentational spacing.
- There should always be a new line at the end of every file.

## Formatting

- Use `'` not `"`.
- Use `//` for comments, not `/* */`.
- Always specify leading 0s, like `0.5`.
- Varibles should be written in [CamelCase](http://en.wikipedia.org/wiki/CamelCase) not [snake_case](http://en.wikipedia.org/wiki/Snake_case).

## Build Process

Projects should always have some form of build process to prepare for deployment. Use [Gulp](http://gulpjs.com) to create a `build` or `deploy` task that minifies and concatenates.

## Tests

Projects must include some form of unit or end to end testing.

- [Mocha](https://github.com/mochajs/mocha)
- [Karma](http://karma-runner.github.io/0.12/index.html)
- [Sinon](http://sinonjs.org/)
- [Chai](http://chaijs.com/)

## Beautiful, spacious syntax.

- Use whitespace to improve readability.
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

## Blocks

## Comments

- Use `//` over `/* ... */`.
- Comments should always be preceded by a blank line.
- Comments start with a capital first letter and when writing a full sentence, end with a `.`.

**Bad**
```
var email;
/* a function */
var send = function(  )
{
	...
}
```

**Good**
```
var email;

// Send the email.
var send = function(  )
{
	...
}
```

## Variables

Always explicitely declare variables.

**Bad**
```

```

**Good**
```

```

## Functions

Express functions as variables.

See squint [func-style](https://github.com/RyanWarner/squint-style/blob/master/docs/javascript-linting-documentatio.md#func-style) linting configuration.

**Bad**
```
function ludacrisSpeed(  )
{
	...
}
```

**Good**
```
var ludacrisSpeed = function(  )
{
	...
};
```

## Comparison Operators

Use `===` and `!==` over `==` and `!=`.

Some people [disagree about this](http://javascriptweblog.wordpress.com/2011/02/07/truth-equality-and-javascript/#more-2108).

> "A strict comparison (e.g., ===) is only true if the operands are of the same type. The more commonly used abstract comparison (e.g. ==) converts the operands to the same Type before making the comparison." 
> 
> See [Comparison operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators) on MDN.


## Conditional Expressions

Don't use shortcuts. Using shortcuts reduces the code's readablitiy.

**Bad** 

Read: "If email do something."
```
if( email )
{
	// something
}
```

**Good**

Read: "If email is not equal to empty, do something."
```
if( email !== '' )
{
	// something
}
```

## Naming Conventions

Code should be as self documenting as possible. This means that names should be descriptive, not cryptic.

**Bad**
```
var gc = function(  )
{
	return c;
}
```

**Good**
```
var getColor = function(  )
{
	return color;
}
```

## Quotes.

Use single quotes `'` not double quotes `"`.

## Commas

Don't use leading commas.

**Bad**
```
var starship =
{
  , class: 'Starfighter'
  , model: 'A-Wing'
  , length: '9.6m'
  , width: '6.48m'
}
```

**Good**
```
var starship =
{
	class: 'Starfighter',
	model: 'A-Wing',
	length: '9.6m',
	width: '6.48m'
}
```

No trailing / dangling commas.

**Bad**
```
var starship =
{
	class: 'Light freighter',
	model: 'Modified YT-1300',
	
}
```

**Good**
```
var starship =
{
	class: 'Light freighter',
	model: 'Modified YT-1300'
}
```

## Semicolons

Always use semicolons. Never rely on [automatic semicolon insertion](http://inimino.org/~inimino/blog/javascript_semicolons) (ASI).

**Bad**
```
var getColor = function(  )
{
	return color
}
```

**Good**
```
var getColor = function(  )
{
	return color;
};
```