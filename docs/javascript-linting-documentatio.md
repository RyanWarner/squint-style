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

See eslint docs for [func-style](http://eslint.org/docs/rules/func-style.html).

## new-cap

`"new-cap": 2`

Constructors should begin with a capital letter.

**Bad**

`var xWing = new starfighter(  );`

**Good**

`var xWing = new Starfighter(  );`

See eslint docs for [new-cap](http://eslint.org/docs/rules/new-cap.html).

## new-parens

`"new-parens": 2`

Constructors should always include `(  )` even if it has no arguments.

**Bad**

`var xWing = new Starfighter`

**Good**

`var xWing = new Starfighter(  )`

See eslint docs for [new-parens](http://eslint.org/docs/rules/new-parens.html).

## space-in-parens

`"space-in-parens": [2, "always"]`

All parenstheses should have have spaces between them, including parens with no arguments.

**Bad**

```
var train = new Train();

doSomething('something');
```

**Good**

```
var train = new Train(  );

doSomething( 'something' );
```

See eslint docs for [space-in-parens](http://eslint.org/docs/rules/space-in-parens.html).