# arithmetic operators



| Operator | Description                                                          |
| -------- | -------------------------------------------------------------------- |
| +        | Addition                                                             |
| -        | Subtraction                                                          |
| \*       | Multiplication                                                       |
| \*\*     | Exponentiation ([ES2016](https://www.w3schools.com/js/js\_2016.asp)) |
| /        | Division                                                             |
| %        | Modulus (Division Remainder)                                         |
| ++       | Increment                                                            |
| --       | Decrement                                                            |



| Operator | Example   | Same As      |
| -------- | --------- | ------------ |
| =        | x = y     | x = y        |
| +=       | x += y    | x = x + y    |
| -=       | x -= y    | x = x - y    |
| \*=      | x \*= y   | x = x \* y   |
| /=       | x /= y    | x = x / y    |
| %=       | x %= y    | x = x % y    |
| \*\*=    | x \*\*= y | x = x \*\* y |

### Adding sring and numbers

`let x = 5 + 5;`\
`let y = "5" + 5;`\
`let z = "Hello" + 5;`\


The result of _x_, _y_, and _z_ will be:

`10`\
`55`\
`Hello5`

``

| Operator | Description                       |
| -------- | --------------------------------- |
| ==       | equal to                          |
| ===      | equal value and equal type        |
| !=       | not equal                         |
| !==      | not equal value or not equal type |
| >        | greater than                      |
| <        | less than                         |
| >=       | greater than or equal to          |
| <=       | less than or equal to             |
| ?        | ternary operator                  |

### JavaScript Type Operators

| Operator   | Description                                                |
| ---------- | ---------------------------------------------------------- |
| typeof     | Returns the type of a variable                             |
| instanceof | Returns true if an object is an instance of an object type |

### JavaScript Bitwise Operators

Bit operators work on 32 bits numbers.

Any numeric operand in the operation is converted into a 32 bit number. The result is converted back to a JavaScript number.

| Operator | Description          | Example | Same as      | Result | Decimal |
| -------- | -------------------- | ------- | ------------ | ------ | ------- |
| &        | AND                  | 5 & 1   | 0101 & 0001  | 0001   |  1      |
| \|       | OR                   | 5 \| 1  | 0101 \| 0001 | 0101   |  5      |
| \~       | NOT                  | \~ 5    |  \~0101      | 1010   |  10     |
| ^        | XOR                  | 5 ^ 1   | 0101 ^ 0001  | 0100   |  4      |
| <<       | left shift           | 5 << 1  | 0101 << 1    | 1010   |  10     |
| >>       | right shift          | 5 >> 1  | 0101 >> 1    | 0010   |   2     |
| >>>      | unsigned right shift | 5 >>> 1 | 0101 >>> 1   | 0010   |   2     |

### Remainder

The **modulus** operator (`%`) returns the division remainder.

#### Example

let x = 5;\
let y = 2;\
let z = x % y`; // z = 2.5`

### Dividing

The **division** operator (`/`) divides numbers.

#### Example

let x = 5;\
let y = 2;\
let z = x / y; // z = 1
