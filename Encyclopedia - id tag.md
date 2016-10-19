# `id` selector

The HTML `id` global attribute allows user to set a unique identifier to any HTML element. There must be only one unique `id` value in the whole HTML document.Its purpose is to identify element when linking, scripting or styling with CSS.


### Syntax 

Setting an `id` value means adding an unique string to an element. It follows a simple rule : <element id="id">

	<body>
		<p id="paragraph">Hello World</p>
	</body>

When invoking to `id` you have to add hash symbol in front of the atrribute value.

	`#paragraph{
		color:red;}`

### Examples

`id` attribute has various uses. Most obvious is to style with CSS your HTML element. The example and syntax is mentioned above.
Another use is to link to an element with a specified `id` within a page:

	<body>
	<h2><a id="top">Heading</a></h2>
	<p>Lots of text....</p>
	<p>Lots of text....</p>
	<a href="#top">Go to top</a>
	</body>

Apart from that it is possible to manipulate elements using unique id's and Java Script. 

	<body>
	<h2><a id="top">Heading</a></h2>
	<p id="first-par">Lots of text....</p>
	<p>Lots of text....</p>
	<a href="#top">Go to top</a>
	</body>

	var paragraph = document.getElementById('first-par');// the variable holds now first p element.


### Naming Rules

An unique id value must contain at least one character,must not contain any space characters. In HTML, all values are case-insensitive

### Special Notes

Using characters except ASCII letters and digits, like '_', '-' and '.' may cause compatibility issues, as they weren't allowed in HTML 4. Though this restriction has been lifted in HTML 5, an `id` should start with a letter.


