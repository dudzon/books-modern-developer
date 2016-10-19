# `:empty` pseudoclass

The `:empty` pseudoclass refers to any HTML element that has no children at all, whitespaces included.A commented element is not considered empty unless there is a whitespace before or after comment.

### Syntax

	:empty {
    //css declarations;
	}

### Examples

Say, there are three divs nested in body element, all having class box.

	<body>
		<div class="box">Lorem ipsum...</div>
		<div class="box"><!-- No content just comment --></div>
		<div class="box">  <!--No content, whitespace before comment--></div>
	</body>

We want to style divs using :empty pseudoclass. 

		.box{
		background-color: red;
		width:100px;
		height:100px;
		}
		.box:empty{
	  	background-color: blue;
		}
		
In this case first div has child element - text  "Lorem ipsum", and third div has a whitespace before comment. That's why both elements have red background-color. Second div is an empty div with no children so it background is blue.

	





