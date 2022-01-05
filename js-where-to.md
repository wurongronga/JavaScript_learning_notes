# JS where to

js can be write in the \<head> and \<body> between \<script>\</script> tags.

script can also be placed in external files:

#### External file: myScript.js

`function myFunction() {`\
&#x20; `document.getElementById("demo").innerHTML = "Paragraph changed.";`\
`}`

`<script src="myScript.js"></script>`



An external script can be referenced in 3 different ways:

* With a full URL (a full web address)
* With a file path (like /js/)
* Without any path
