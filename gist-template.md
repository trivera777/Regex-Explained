## Regex Explained
Short for regular expressions, regex are a series of special characters that define a search pattern.

## Summary
In this gist I will explain how regex is used to match emails using the expression `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`.
<!-- Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.
 -->
 
## Table of Contents
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
The components of a regex include achors, which are the characters `^` and `$`. 

Both anchors together are used to test whether or not a string fully mathes the pattern.

The `^` anchor signifies the beginning of the string.

While the `$` anchor signifies the end of the string.

Check out this example.

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

### Quantifiers
The final component of a regex are quantifiers.

Did you notice this part of the string, `{2,6}`? That is a quantifier. 

A quantifier sets the limit of the string that the regex matches.

The number `2` in this case is the minimum and `6` is the maximum number of characters that the regex is looking for.

In other words, the string has to be between `2` and `6` characters long.

### Grouping Constructs

### Bracket Expressions
Brackets inidcate a set of characters to match.

`/^([a-z0-9])$/`

Below is a good example to further break down bracket expressions,

`'elephant'.match(/[a-d]/) // -> matches 'a'`

`'elephant'.match(/[A-D]/) // -> no match`

Character sets are case sensitive, unless the `i` flag is set,

`'elephant'.match(/[A-D]/i) // -> matches 'a'`

### Character Classes
Character classes remove anything that's not a number.

Some of these character classes are:

`\d` - any digit from `0` to `9`.

`\s` - any space, including tabs and line breaks.

`\w` - any "wordly" character, from the basic Latin alphabet, including the underscore `_`.

Here is an example:

`let str = "Is there CSS4?";`

`let regexp = /CSS\d/`

`alert( str.match(regexp) ); // CSS4`


### The OR Operator

### Flags
Flags define additional funcationality or limits for the regex.

The three most common flags are 

`g` - Gobal Search: regex should be testeeed against all possible matches.

`i` - Case-Insensitive Search: case will be ignored while attempting to match.

`m` - Multi-Line Search: will be treated as multiple lines.

### Character Escapes
The backslash `\` is a regex escape character.

To reference a literal character, you must escape it within the regular expressiion.

Example:

`/\?/` - will find the literal character `?`.

## Author

<hr/>
<p align="center">
  <a href="mailto:trivera51580@gmail.com?subject=Hello%20Tifanny%20Rivera"><img src="https://img.shields.io/badge/gmail-%23D14836.svg?&style=for-the-badge&logo=gmail&logoColor=white" /></a>&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://www.facebook.com/tifanny.rivera777/"><img src="https://img.shields.io/badge/facebook-%233B5998.svg?&style=for-the-badge&logo=facebook&logoColor=white" /></a>&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://www.instagram.com/tifann_y/"><img src="https://img.shields.io/badge/instagram-%23dc2743.svg?&style=for-the-badge&logo=instagram&logoColor=white" /></a>&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://www.linkedin.com/in/tifannyrivera/"><img src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" /></a>&nbsp;&nbsp;&nbsp;&nbsp;
</p>
<hr/>
