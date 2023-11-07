# HTML-list-from-indented-text

Converts a string containing indents - by space and linefeed characters - to an HTML entity erected by ul lists.
Type/edit a text and call the function with your text being transferred as a string.
While typing/editing your text:
	- As a rule of indentation, all elements within the same level should start with the same number of space characters.
	- To have a new paragraph within the current element, start the new paragraph with just a linefeed followed by no space character.
	- To end the indentation and return to the base text level, append a space character to the last paragraph of the indentation.
		- You don't need to append a space character to end the indentation at the end of the text in cases where the text does not end with a base text level.
	- For visual purposes, you can add a hyphen following the space characters at the beginning of the paragraphs.
Example 1: two-level indentation
			base text paragraph
			 -indented paragraph, level 1, element 1
			 -indented paragraph, level 1, element 2
			  -indented paragraph, level 2, element 1
Example 2: additional paragraphs within an element
			base text paragraph
			 -indented paragraph, level 1, element 1
			second paragraph of level 1, element 1
			third paragraph of level 1, element 1
			 -indented paragraph, level 1, element 2
Example 3: ending indentation
			base text paragraph
			 -indented paragraph, level 1, element 1
			 -indented paragraph, level 2, element 1 <<< HERE IS A SPACE CHARACTER
			base text paragraph
