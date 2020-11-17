# Typeof
```js
let v;
typeof v //"undefined"

v = "1";
typeof v //"string"

v = 1;
typeof v //"number"

v = true;
typeof v //"boolean"

v = {};
typeof v //"object"

v = Symbol();
typeof v //"symbol"
```

## Notes
- typeof returns a string....always
  - returns an option from an enum list
  - typeof CANNOT return anything accept a string


## Gotchas
```js
// bug 1
let v = null;
typeof v //returns..."object"

// bug 2
v = function(){}
typeof v //returns... "function"?!

// bug 3
v = [2,3,4,5]
typeof v //returns... "object"?!
```

### Bug 1
- ... its a bug! it should return `"null"`

### bug 2
- ... not REALLY a primitive type

### bug 3
- can use v.isArray() to see if it is an array