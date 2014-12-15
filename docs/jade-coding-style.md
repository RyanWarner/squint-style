
# Jade Coding Style

To my knowledge, there is no Jade linter available. Despite this, it is still important to keep a consistent style when writing Jade.

## Quotes

Consistent with JavaScript, always use single quotes.

**Bad**

`a( href="http://squint-style.guide" )`

**Good**

`a( href='http://squint-style.guide' )`

## Plain Text

Even with syntax highlighting, text can sometimes blend in with the tag or atributes. For readability, always place piped text on a new line.

**Bad**

`p I went for a Sunday jog.`

**Good**

```
p
    | I went for a Sunday jog.
```

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


## Space Inside Parenthesis

There should always be a single space inside parenthesis.

**Bad**

`a(href="http://squint-style.guide")`

**Good**

`a( href='http://squint-style.guide' )`

## 

## Class and ID Declarations

Wherever possible, favor literal syntax as opposed to attributes.

**Bad**

`div( class='avatar' )`

`div( id='content' )`

**Good**

`.avatar`

`#content`
 
## Commas Between Attributes
 
For reabability, always put a comma between attribute definiteions.
 
**Bad**
 
`input( type='range' min='0' max='100' )`

**Good**
 
 `input( type='range', min='0', max='100' )`