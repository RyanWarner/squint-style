# JavaScript Linters

This file attmepts to make note of important linters in squint-style. It does not address every linter. If you want to see all of them, read the [entire list of eslint rules](http://eslint.org/docs/rules/).

- 0 - turn the rule off
- 1 - turn the rule on as a warning (doesn't affect exit code)
- 2 - turn the rule on as an error (exit code is 1 when triggered)

See [eslint configuration docs](http://eslint.org/docs/configuring/).

## brace-style

`"brace-style": 0`

Brace style is turned off because eslint does not support enforcing Allman style indentation / brace style.

See eslint docs for [brace-style](http://eslint.org/docs/rules/brace-style.html).

## func-style

`"func-style": [2, "expression"]`

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