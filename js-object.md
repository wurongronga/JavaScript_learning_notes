# JS object

### Object Definition

You define (and create) a JavaScript object with an object literal:

`const person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};`

{% hint style="info" %}
JavaScript objects are containers for **named values** called properties.
{% endhint %}

### Object Properties

The **name:values** pairs in JavaScript objects are called **properties**:

| Property  | Property Value |
| --------- | -------------- |
| firstName | John           |
| lastName  | Doe            |
| age       | 50             |
| eyeColor  | blue           |

real world object

| Object                                                | Properties                                                                                           | Methods                                                                        |
| ----------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| ![](https://www.w3schools.com/js/objectExplained.gif) | <p><br>car.name = Fiat<br><br>car.model = 500<br><br>car.weight = 850kg<br><br>car.color = white</p> | <p><br>car.start()<br><br>car.drive()<br><br>car.brake()<br><br>car.stop()</p> |

### Object Methods

A method is a function stored as a property.

```
const person = {
  firstName: "John",
  lastName : "Doe",
  id       : 5566,
  fullName : function() {
    return this.firstName + " " + this.lastName;
  }
};
```

### The **this** Keyword

In a function definition, `this` refers to the "owner" of the function.

In the example above, `this` is the **person object** that "owns" the `fullName` function.

In other words, `this.firstName` means the `firstName` property of **this object**.



### Accessing Object Methods

You access an object method with the following syntax:

_`objectName.methodName()`_

<mark style="background-color:orange;">If you access a method</mark> <mark style="background-color:orange;"></mark><mark style="background-color:orange;">**without**</mark> <mark style="background-color:orange;"></mark><mark style="background-color:orange;">the () parentheses, it will return the</mark> <mark style="background-color:orange;"></mark><mark style="background-color:orange;">**function definition**</mark><mark style="background-color:orange;">:</mark>

#### Example

name = person.fullName;

### Do Not Declare Strings, Numbers, and Booleans as Objects!

When a JavaScript variable is declared with the keyword "`new`", the variable is created as an object:

```
x = new String();        // Declares x as a String object
y = new Number();        // Declares y as a Number object
z = new Boolean();       // Declares z as a Boolean object
```

Avoid `String`, `Number`, and `Boolean` objects. They complicate your code and slow down execution speed.
