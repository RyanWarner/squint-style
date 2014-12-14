
# Jade Coding Style

While there is no Jade linter that I know of, we should make it our responsibillity to follow these guidelines when writing Jade templates.

## Quotes

Consistent with JavaScript, always use single quotes.

**Bad**

`a( href="http://squint-style.guide" )`

**Good**

`a( href='http://squint-style.guide' )`

## Plain Text

Use piped text on a new line. Being consistent with plain text location makes it easier to find and change. Sometimes element attribute lines in combination with plain text can get unweildy.

**Bad**

`p I went for a Sunday jog.`

**Good**

```
p
    | I went for a Sunday jog.
```

## Space Inside Parenthesis

There should always be a single space inside parenthesis.

**Bad**

`a(href="http://squint-style.guide")`

**Good**

`a( href='http://squint-style.guide' )`

## Class and ID Declarations

Wherever possible, favor literal syntax as opposed to attributes.

**Bad**

`div( class='avatar' )`

`div( id='content' )`

**Good**

`.avatar`

`#content`

## Block Expansion

Don't use block expansion. Saving space is only helpful if it makes the code more readable. It is much easier to use indentation to visually differentiate children and their parents.

**Bad**

`div: span Hello World`

**Good**

```
div
    span
        | Hello World
 ```