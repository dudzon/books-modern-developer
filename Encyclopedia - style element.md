# `style` element

The HTML `style` element allows user to add CSS styles directly in HTML file. The style information can  be embed  either in `head` section  of your HTML file or in HTML markup between other tags<br>

Examples: 

`style` element in head section.

	<!DOCTYPE html>
	<html lang="en">
	<head>
	<meta charset="UTF-8">
	<title>Document</title>
	<style type="text/css">
		body{background-color:red;}
	</style>
	</head>

`style` in HTML markup.

	<body>
	<style type="text/css">
		p{
			color:green;
		}
	</style>
	<p>Lorem Ipsum...</p>
	</body>

### Syntax

Typical HTML syntax where neither tag is ommissible. `<style>Your CSS code...</style>`

### Attributes

`type` - this attribute defines the styling language.This attribute is optional and by default is set to `text/css`

`media` - this attribute which media the style should apply to. If the attribute is missing its value is set to all. Other media types :<br>
aural | Intended for speech synthesizers.<br>
braille | Intended for braille tactile feedback devices.<br>
embossed | Intended for paged braille printers.<br>
handheld | Intended for handheld devices.<br>
print | Intended for paged, opaque material and for documents viewed on screen in print preview mode<br>
projection | Intended for projected presentations, for example projectors or print to transparencies.<br>
screen | Intended primarily for color computer screens.<br>
tty | Intended for media using a fixed-pitch character grid, such as teletypes, terminals, or portable devices with limited display capabilities.<br>
tv | Intended for television-type devices <br>

`scoped` - It allows to apply style only to its parent element. If  the attribute is absent, the style applies to the whole document.

Example:

 	<section>
	<p>This should be also red</p>
    <style scoped>
      p { color: red; }
    </style>
    <p>This is paragraph and it is red.</p>
  	</section>

`title` - specifies alternative style sheet sets.


### Special Notes

`scoped` attribute is not supportes by Internet Explorer, Safari and Opera. It works only in Firefox and Chrome


