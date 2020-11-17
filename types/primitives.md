# Primitive Types
"In JS, everything is an object".
NOT TRUE!!! (_false, haha_)
- [JS Ecma Spec on Types](https://tc39.es/ecma262/#sec-ecmascript-data-types-and-values)

## A Type
A Type is a set of characteristictis && behaviors that we expect to access && use with a value

## Types, a list 
- undefined
- null
- boolean
- string
- symbol
- number
- object

### Undefined
- one value `undefined`

### String
- "string literal"

### Number
- all of js numbers **

### Boolean
- `true` or `false`
- note, they behave differently

### Object
- many things BEHAVE as an object that are NOT objects

### Symbols

### BigInt
```js
const thisThing = 42n;
typeof 42n //returns BigInt
```

## Non-Types
- undeclared
- null
  - its a bug
- functions
- array
  - numerically indexed
  - various methods
  - its like an object, sort-of a 'sub-type'
- bigint



## Undefined vs Undeclared

### Undeclared
- never been created

### Undefined
- def a var, currenlty no value tho

## NaN && isNaN
```js
const thisNum = Number("0o41") // Octal representation of 34, returns 34
const thisNextAge = Number("35") // returns 35
const nonAge = Number("n/a") // returns NaN
const stringAge = Number("String Age") // NaN

```
### NaN
- Not a Number...sort-of
- REALLY
  - an invalid number
### isNaN