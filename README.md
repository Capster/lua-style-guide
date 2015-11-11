# Lua Style Guide

<a name="code_layout"/>
## Code layout

<a name="tabs_or_spaces"/>
### Tabs or Spaces?

Use **tabs only**. Never mix tabs and spaces.

<a name="maximum_line_length"/>
### Maximum Line Length

Limit all lines to a maximum of 79 characters.

<a name="blank_lines"/>
### Blank Lines

Separate top-level function and class definitions with a single blank line.

Use a single blank line within the bodies of methods or functions in cases where this improves readability.

<a name="trailing_whitespace"/>
### Trailing Whitespace

Do not include trailing whitespace on any lines.

<a name="encoding"/>
### Encoding

UTF-8 is the preferred source file encoding.

<a name="whitespace"/>
## Whitespace in Functions and Operators

Avoid extraneous whitespace in the following situations:

- Immediately inside parentheses, brackets or braces

	```lua
	print('argument') -- Yes
	print( 'argument' ) -- No
	```
- Immediately before a comma

	```lua
	print(x, y) -- Yes
	print(x , y) -- No
	```

- Always surround these binary operators with a single space on either side
	- assignment: `=`
	- comparisons: `==`, `<`, `>`, `<=`, `>=`, `!=`, `~=` etc.
	- arithmetic operators: `+`, `-`, `*`, `/`, etc.
	- _(Do not use more than one space around these operators)_

	```lua
	-- Yes
	x = 1
	y = 1
	steamID = 3

	-- No
	x      	= 1
	y      	= 1
	steamID = 3
	```

<a name="naming"/>
## Naming Conventions

Use `camelCase` (with a leading lowercase character) to name all local variables.

Use `CamelCase` (with a leading uppercase character) to name all global variables, fields and methods.

For enums, use all uppercase with underscores: `ENUM_LIKE_THIS`.

<a name="comments"/>
## Comments

The first word of the comment should be capitalized, unless the first word is an identifier that begins with a lower-case letter.
If a comment is short, the period at the end can be omitted.

<a name="block_comments"/>
### Block Comments

Block comments apply to the block of code that follows them.

Paragraphs inside of block comments are separated by a single line.

```lua
--[[
	Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
	tempor incididunt ut labore et dolore magna aliqua.

	Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
	tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
	quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
	consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
	cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
	proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
]]

Init()
Start()
Stop()
```

<a name="inline_comments"/>
### Inline Comments

All inline comments should start with a `--` and a single space.

The use of inline comments should be limited, because their existence is typically a sign of a code smell.

```lua
x = x + 1 # One second prediction
```

<a name="strings"/>
## Strings

Prefer single quoted strings (`''`) instead of double quoted (`""`) strings, unless features like string interpolation are being used for the given string.

<a name="misc"/>
## Miscellaneous

`and` is preferred over `&&`.

`or` is preferred over `||`.

`not` is preferred over `!`.

`!=` is preferred over `~=`.
