# Lua Style Guide

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

## Naming Conventions

Use `camelCase` (with a leading lowercase character) to name all local variables.

Use `CamelCase` (with a leading uppercase character) to name all global variables, fields and methods.

For enums, use all uppercase with underscores: `ENUM_LIKE_THIS`.
