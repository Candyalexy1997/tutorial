# Title (replace with your title)

This tutorial will explain and define the sequence of special characters to verify a search term, specifically a Hex (shown below):

Hex: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/


## Summary

I will be discuss and break down the parts of a regular expression used to match Hex Values. Hex values are mostly used for color using the hexadecimal color code format. 

For styling you can use the hex triplet to represent colors on a webpage. There are two formats : a standard hex triplet and a shorthand hex format, both of these formats start with a #.

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
Anchors belong to the family of regex tokens that don't match any characters, but that assert something about the string or the matching process. Anchors assert that the engine's current position in the string matches a well-determined location: for instance, the beginning of the string, or the end of a line.

The (^) character represents the beginning of any position.
The ($) character represents the end of the string, or the end of a line if the multiline flag (m) is enabled.

(\b) word boundary is a position between a word character and non-word character or position.

(\B) Matches any position that is not a word boundary.

### Quantifiers

Quantifiers are used to quantify how many times a part of your regular expression should be repeated.  Every time you want to repeat something in a regex  you can write a quantifier after it to specify how many times it should be repeated.

Quantifiers are shown below based on the Hex Regex. 

? is syntax sugar for {0,1}
+ is syntax sugar for (1)
{N} - N is a positive integer


### OR Operator

OR Operator: |

Code Snipet: [a-f0-9]{6}|[a-f0-9]{3}

Description: The | indicator is a boolean that matches either the expression before or after.


### Character Classes

Code Snipet: a-f0-9 Description: 

Character classes only matches one out of several characters defined in the character set. A hyphen can be used inside a character class to define a range of characters More than one range can be used -- as is the case in our code snipet.

Example: [0-9] This character class matches a single digit between 0 and 9

In the case above -  the character class consists of lower case a-f and/or integer 0-9

### Flags

### Grouping and Capturing

The () groups the regular expression between them. The grouping treats multiple characters as a single unit. This can proof useful when extracting information using any programming language. This group of data will be exposed in the form of an array. Values can be accessed using an index on the result of the match.

For the Hex example, the grouped expression is a bracket expression whose details are provided in the section below. Ultimately the end string anchor $ is applied to this grouping.

### Bracket Expressions

Bracket Expression: []

Code Snipet: [a-f0-9]

Bracket expression is a regex that will match a specific pattern of characters (alphabetic, numeric, special characters, symbols etc..) defined within the brackets

In our reg ex, the bracket [] expression indicates matching a string that has any lower case character between a-f or any integer between 0-9


### Greedy and Lazy Match

Quantifier: {}

Greedy means match the longest possible string. Lazy means match the shortest possible string.

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

My name is Candice, I am new to programming and still continuing to learn more each and every day.  

Github: https://github.com/Candyalexy1997