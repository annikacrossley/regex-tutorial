# Matching a Hex Value 

A regex is a "regular expression", which means a series of characters that define a search pattern. These are useful in JavaScript and though they may not make sense at first glance, different regexs can be used to verify user input such as a username, email, URL, HTML, or as we will review today: a hex value. 

## Summary

Hexadecimal codes, or hex codes, are used to refer to colors. Like most information used to communicate with our computers, a hex code needs to be in a certain format. This includes starting with a "#" symbol, consisting of letters A thru F and numbers 0-9, and be either 3 or 6 characters long. The following regex verifies that the input provided to identify a hex code meets these criteria: <br>

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/ `

In this tutorial we will explain why and how this regex works. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

A regex is wrapped in slashes ('/') because it is a literal (a fixed value in JavaScript). If we look at our hex matching regex, we can see that it is wrapped in slashes: 
<br>

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` 

Next, we will examine the anchors of the hex value regex. 

### Anchors

An anchor is represented by two characters: `^` to signify the beginning of the phrase and `$` to signify the end. In our regex, we can see the first characters inside the slashes are these anchors.

Next, we will discuss what the sections between our anchors mean. 

### Quantifiers
The next characters after our first anchor is called a quantifier. In our expression, the quantifier is `?` that comes after the symbol `#`. This quantifier `?` means that there will be either 0 or 1 characters after the symbol `#`. 

So far, we have discussed the beginning `/^#?` and the end `$/` of our regex. Next, we will break down the middle sections that are housed within the parentheses: <br> `([a-f0-9]{6}|[a-f0-9]{3})`

### OR Operator
To best break down the remaining sections of our regex, we can start at the OR Operator. This is signified by the OR operator symbol: `|`. This means that our expression is looking for either `[a-f0-9]{6}` or `[a-f0-9]{3}`. 

In the following sections we will learn how each of those phrases define and identify a hex code. 

### Character Classes
In our regex, we see character classes twice. This first is `a-f` and the second is `0-9`. This means that we are looking for characters `a-f` (a, b, c, d, e, or f) and `0-9` (0, 1, 2, 3, 4, 5, 6, 7, 8, or 9). 

Remember, a hex code contains letters A-F and numbers 0-9. Our character classes define that. 

### Grouping and Capturing
Grouping is represented by parentheses. As mentioned before, a portion of our hexadecimal regex is housed within parentheses: <br> `([a-f0-9]{6}|[a-f0-9]{3})`

The characters within the parntheses is considered a group. By making this portion a group, it separates the phrase to act as literal characters. 

### Bracket Expressions
On each side of our OR Operator `|`, we have a bracket expression: `[a-f0-9]`

This bracket expression contains our character classes that we discussed earlier.  

## Author

Annika Crossley is the author of this tutorial. She is a web development student in the UW Full Stack Development bootcamp. Please explore her work on <a href="https://github.com/annikacrossley">Github</a>.


