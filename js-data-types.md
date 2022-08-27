# JS data types

## JavaScript Primitive vs. Reference Values

* Primitive values ([null](https://www.javascripttutorial.net/object/javascript-null/), [undefined](https://www.javascripttutorial.net/javascript-undefined/), [boolean](https://www.javascripttutorial.net/javascript-boolean-type/), [number](https://www.javascripttutorial.net/javascript-number/), [string](https://www.javascripttutorial.net/string/), [symbol](https://www.javascripttutorial.net/es6/symbol/), and [BigInt](https://www.javascripttutorial.net/es-next/javascript-bigint/))
* Reference values that refer to objects.

JavaScript variables can hold different data types: numbers, strings, objects and more:

let length = 16;                               // Number\
let lastName = "Johnson";                      // String\
let x = {firstName:"John", lastName:"Doe"};    // Object

{% hint style="info" %}
When adding a number and a string, JavaScript will treat the number as a string.
{% endhint %}

JavaScript evaluates expressions from left to right. Different sequences can produce different results:

#### JavaScript:

let x = 16 + 4 + "Volvo";

Result:

`20Volvo`

#### JavaScript:

let x = "Volvo" + 16 + 4;

Result:

`Volvo164`

### JavaScript Types are Dynamic

JavaScript has dynamic types. This means that the same variable can be used to hold different data types:

#### Example

let x;           // Now x is undefined\
x = 5;           // Now x is a Number\
x = "John";      // Now x is a String

### JavaScript Strings

A string (or a text string) is a series of characters like "John Doe".

Strings are written with quotes. You can use single or double quotes

You can use quotes inside a string, as long as they don't match the quotes surrounding the string

### JavaScript Numbers

JavaScript has only one type of numbers.

Numbers can be written with, or without decimals

Extra large or extra small numbers can be written with scientific (exponential) notation

### Undefined

In JavaScript, a variable without a value, has the value `undefined`. The type is also `undefined`.

#### Example

let car; // Value is undefined, type is undefined

Any variable can be emptied, by setting the value to `undefined`. The type will also be `undefined`.

#### Example

car = undefined;    // Value is undefined, type is undefined
