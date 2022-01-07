# JS event

HTML events are **"things"** that happen to HTML elements.

When JavaScript is used in HTML pages, JavaScript can **"react"** on these events.



### HTML Events

An HTML event can be something the browser does, or something a user does.

Here are some examples of HTML events:

* An HTML web page has finished loading
* An HTML input field was changed
* An HTML button was clicked

_JavaScript lets you execute code when events are detected._

HTML allows event handler attributes, **with JavaScript code**, to be added to [HTML elements](html-element.md).

With single quotes:

<_element_ _event_=**'**_**some JavaScript**_**'**>

With double quotes:

<_element_ _event_=**"**_**some JavaScript**_**"**>



In the following example, an `onclick` attribute (with code), is added to a `<button>` element:

#### Example

```
<button onclick="document.getElementById('demo').innerHTML = Date()">The time is?</button>
```

{% hint style="info" %}
JavaScript code is often several lines long. It is more common to see event attributes calling functions:
{% endhint %}

#### Example

\<button onclick="displayDate()">The time is?\</button>



### Common HTML Events

Here is a list of some common HTML events:

| Event       | Description                                        |
| ----------- | -------------------------------------------------- |
| onchange    | An HTML element has been changed                   |
| onclick     | The user clicks an HTML element                    |
| onmouseover | The user moves the mouse over an HTML element      |
| onmouseout  | The user moves the mouse away from an HTML element |
| onkeydown   | The user pushes a keyboard key                     |
| onload      | The browser has finished loading the page          |
