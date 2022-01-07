# JS strings

### String Length

let text = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";&#x20;

let length = text.length;



### Escape Character

| Code | Result | Description  |
| ---- | ------ | ------------ |
| \\'  | '      | Single quote |
| \\"  | "      | Double quote |
| \\\\ | \\     | Backslash    |

Six other escape sequences are valid in JavaScript:

| Code | Result               |
| ---- | -------------------- |
| \b   | Backspace            |
| \f   | Form Feed            |
| \n   | New Line             |
| \r   | Carriage Return      |
| \t   | Horizontal Tabulator |
| \v   | Vertical Tabulator   |

### Breaking Long Code Lines

For best readability, programmers often like to avoid code lines longer than 80 characters.

If a JavaScript statement does not fit on one line, the best place to break it is after an operator:

#### Example

document.getElementById("demo").innerHTML =\
"Hello Dolly!";

You can also break up a code line **within a text string** with a single backslash: (not recommand)

#### Example

document.getElementById("demo").innerHTML = "Hello \\\
Dolly!";

{% hint style="info" %}
The `\` method is not the preferred method. It might not have universal support.\
Some browsers do not allow spaces behind the `\` character.
{% endhint %}

A safer way to break up a string, is to use string addition:

#### Example

document.getElementById("demo").innerHTML = "Hello " +\
"Dolly!";

You cannot break up a code line with a backslash:

#### Example

document.getElementById("demo").innerHTML = \\\
"Hello Dolly!";



Don't use string object. String objects can produce unexpected results:

When using the `==` operator, x and y are **equal**:

let x = "John";\
let y = new String("John");

When using the `===` operator, x and y are **not equal**:

let x = "John";\
let y = new String("John");

{% hint style="info" %}
JavaScript objects cannot be compared.

`(x == y)` true or false?

let x = new String("John");\
let y = new String("John");

`(x === y)` true or false?

let x = new String("John");\
let y = new String("John");



//false false

Comparing two JavaScript objects **always** returns **false**.
{% endhint %}



