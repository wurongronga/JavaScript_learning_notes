# JS const, let, var

Variables defined with `const` cannot be Redeclared.

Variables defined with `const` cannot be Reassigned.

Variables defined with `const` have Block Scope.

|   |                                             |                                                          |                                                           |
| - | ------------------------------------------- | -------------------------------------------------------- | --------------------------------------------------------- |
|   | const                                       | let                                                      | var                                                       |
|   | cannot be redeclared                        | cannot be redeclared                                     | can be redeclared                                         |
|   | cannot be reassigned                        | can be reassigned                                        | can be reassigned                                         |
|   | block scope                                 | block scope                                              | global scope                                              |
|   | must be assigned when declared              | must be declared before use                              | can use the variable before it is declared                |
|   | defines a constant reference to a value     | assign value to a variable                               | assign value to a variable                                |
|   | **hoisted** to the top, but not initialized | **hoisted** to the top of the block, but not initialized | **hoisted** to the top and can be initialized at any time |

{% hint style="info" %}
redecaring a variable using var keyword can impose problems

Redeclaring a variable inside a block will also redeclare the variable outside the block:

`var x = 10; // Here x is 10`

`{ var x = 2; // Here x is 2 }`

`// Here x is 2`

Redeclaring a variable using the `let` keyword can solve this problem.

Redeclaring a variable inside a block will not redeclare the variable outside the block:

`let x = 10; // Here x is 10`

`{ let x = 2; // Here x is 2 }`

`// Here x is 10`
{% endhint %}



{% hint style="info" %}
With `let`, redeclaring a variable in the same block is NOT allowed:

``

`var x = 2; // Allowed let x = 3; // Not allowed`

`{ let x = 2; // Allowed let x = 3 // Not allowed }`

`{ let x = 2; // Allowed var x = 3 // Not allowed }`
{% endhint %}

### Let Hoisting

Variables defined with `var` are **hoisted** to the top and can be initialized at any time.

Meaning: You can use the variable before it is declared:

This is OK:

`carName = "Volvo";`&#x20;

`var carName;`

Variables defined with `let` are also hoisted to the top of the block, but not initialized.

Meaning: <mark style="background-color:orange;">Using a</mark> <mark style="background-color:orange;"></mark><mark style="background-color:orange;">`let`</mark> <mark style="background-color:orange;"></mark><mark style="background-color:orange;">variable before it is declared will result in a</mark> <mark style="background-color:orange;"></mark><mark style="background-color:orange;">`ReferenceError`</mark>:

#### Example

`carName = "Saab";`\
`let carName = "Volvo";`

``

### Constant Objects and Arrays

The keyword `const` is a little misleading.

It does not define a constant value. It defines a constant reference to a value.

Because of this you can NOT:

* Reassign a constant value
* Reassign a constant array
* Reassign a constant object

But you CAN:

* Change the elements of constant array
* Change the properties of constant object

Redeclaring a variable with `const`, in another scope, or in another block, is allowed:

#### Example

const x = 2;       // Allowed\
\
{\
&#x20; const x = 3;   // Allowed\
}\
\
{\
&#x20; const x = 4;   // Allowed\
}
