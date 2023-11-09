# HTML-list-from-indented-text

Converts a string containing indents - by space and linefeed characters - to an HTML entity erected by ul lists.
Type/edit a text and call the function with your text being transferred as a string.
While typing/editing your text:
	- As a rule of indentation, all elements within the same level should start with the same number of space characters.
	- To have a new paragraph within the current element, start the new paragraph with just a linefeed and prepend no space character.
	- To quit the indentation, append a space character to the last paragraph of the indentation.
		- You don't need to append a space character in cases where the whole text ends with the end of the indentation.
	- For visual purposes, you can add a hyphen following the space characters at the beginning of the indented paragraphs.
Example 1: two-level indentation
			base-text paragraph
			 -indented paragraph, level 1, element 1
			 -indented paragraph, level 1, element 2
			  -indented paragraph, level 2, element 1
Example 2: additional paragraphs within an element
			 -indented paragraph, level 1, element 1
			second paragraph of level 1, element 1
			third paragraph of level 1, element 1
			 -indented paragraph, level 1, element 2
Example 3: ending indentation
			 -indented paragraph, level 1, element 1
			 -indented paragraph, level 2, element 1 <<< HERE IS A SPACE CHARACTER
			base-text paragraph
