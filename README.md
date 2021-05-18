# BasicAndWeirdStuffAboutJS

> true && expression = expression

``` 
Example: (2>1) && (1+3)  = 4 
```

> false && expression = false

``` 
Example : (1>2) && (1+3) = false
```

> 0 && expression = 0
```
let count = 0
count && "hello" = 0 
```
> Computed Property Names
##### [MDN Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Object_initializer#computed_property_names)
```
// Computed property names (ES2015)
let i = 0
let a = {
  ['foo' + ++i]: i,
  ['foo' + ++i]: i,
  ['foo' + ++i]: i
}

console.log(a.foo1) // 1
console.log(a.foo2) // 2
console.log(a.foo3) // 3

const items = ["A","B","C"];
const obj = {
[items]: "Hello"
}
console.log(obj); // A,B,C: "Hello"
console.log(obj["A,B,C"]) // "Hello"

let param = 'size'
let config = {
  [param]: 12,
  ['mobile' + param.charAt(0).toUpperCase() + param.slice(1)]: 4
}

console.log(config) // {size: 12, mobileSize: 4}
```
