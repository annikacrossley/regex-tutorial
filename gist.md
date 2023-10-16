# Matching a Hex Value 

A regex is a "regular expression", which means a series of characters that define a search pattern. These are useful in JavaScript and though they may not make sense at first glance, different regexs can be used to verify user input such as a username, email, URL, HTML, or as we will review today: a hex value. 

## Summary

Hexadecimal codes, or hex codes, are used to refer to colors. Like most information used to communicate with our computers, a hex code needs to be in a certain format. This includes starting with a "#" symbol, consisting of letters A thru F and numbers 0-9, and be either 3 or 6 characters long. The following regex verifies that the input provided to identify a hex code meets these criteria: 
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/ 

In this tutorial we will explain why and how this regex works. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

### Quantifiers

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
