# HTML-list-from-indented-text-VBScript-

Converts a string containing indents - by space and linefeed characters - to an HTML entity erected by ul lists.
Type/edit a text and call the function with your text being transferred as a string.
While typing/editing your text:
	- As a rule of indentation, all elements within the same level should start with the same number of space characters.
	- To have a new paragraph within the current element, start the new paragraph with just a linefeed followed by no space character.
	- To end an indent level, append a space character to the paragraph that corresponds to the last element or paragraph of that level.
		- To which level the next paragraph is to belong will be, as a rule of indentation, determined by the number of prepended space characters.
	- For visual purposes, you can add a hyphen following the space characters at the beginning of the paragraphs.
Example 1: two-level indentation
			base text paragraph
			 -indented paragraph, level 1, element 1
			 -indented paragraph, level 1, element 2
			  -indented paragraph, level 2, element 1
Example 2: two paragraphs within an element
			base text paragraph
			 -indented paragraph, level 1, element 1
			second paragraph of level 1, element 1
			 -indented paragraph, level 1, element 2
Example 3: ending a level and returning to the base text level
			base text paragraph
			 -indented paragraph, level 1, element 1
			 -indented paragraph, level 2, element 1 <<< HERE IS A SPACE CHARACTER
			base text paragraph
Example 4: ending a level and returning to the second previous level
			base text paragraph
			 -indented paragraph, level 1, element 1
			  -indented paragraph, level 2
			   -indented paragraph, level 3 <<< HERE IS A SPACE CHARACTER
			 -indented paragraph, level 1, element 2
