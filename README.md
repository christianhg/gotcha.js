# gotcha.js 💣

> A collection of counter-intuitive *gotchas* in JavaScript.

### Automatic Type Conversion

JavaScript facilitates *type coercion* as a nifty trick to quietly convert "wrong" values given to a program.

```js
undefined == null
// => true

[] + 42
// => '42'

{} + {}
// => '[object Object][object Object]'

true == 1
// => 1

'4' + 2
// => '42'

'4' - 2
// => 2

'4' * 2
// => 8

42 * null
// => 0
```

To prevent unexpected type conversions in equality checks, the `===` and `!==` operators are often used in favor of `==` and `!=`.
