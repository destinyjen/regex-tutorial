# Title 

Regex Tutorial

## Summary

A regex, which is short for regular expression, is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They allow you to define complex search patterns that can be incredibly powerful in data validation, text processing, and more examples.

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

/^[\w.-]+@[a-zA-Z]+\.[a-zA-Z]{2,}$/

### Anchors

Regex anchors are components that define the position in the string where a match should occur. They do not match any characters themselves but rather specify where in the string the pattern should be found. The two main regex anchors are:

^ (caret): This anchor matches the start of a line. It ensures that the pattern following the caret is found at the beginning of a line.

$ (dollar sign): This anchor matches the end of a line. It ensures that the pattern preceding the dollar sign is found at the end of a line.

Again, anchors specify positions in the text where matches must occur, such as ^ for the start of the line and $ for the end of the line. This essentially closes in the code inside the regex line. 

### Quantifiers

Quantifiers are symbols that specify the quantity of characters or groups in a regular expression pattern. They control how many times a character or group can appear in the input text, like + for one or more occurrences and * for zero or more. Here we only use plus becaus ethere are several components we need included within an email address. 

### Grouping Constructs

Grouping constructs are used to group multiple characters or subpatterns together in a regular expression. They are enclosed within parentheses ( and ). Grouping constructs serve several purposes in regex( ) are used to create subexpressions within a larger regex, allowing you to apply quantifiers or capture matches.

### Bracket Expressions

Regex bracket expressions, also known as character classes, are used in regular expressions to match a single character out of a set of characters. They allow you to specify a range or a list of characters that you want to match at a specific position in the input text. Bracket expressions [ ] define sets of characters to match against, such as [a-z] for any lowercase letter or [0-9] for any digit. We use these to define the parameters of the characters within each email address.

### Character Classes

Regex character classes, also known as character sets or character ranges, are used in regular expressions to match a single character from a specific set of characters. They provide a way to define a group of characters that can be matched at a particular position in the input text. Character classes \d, \w, and \s match digits, word characters, and whitespace respectively, providing shorthand for common character sets. We use \w for word characters to be included in the email address. 

### The OR Operator

The OR operator in regex, represented by the vertical bar |, allows you to specify alternatives within a regular expression pattern. It is used to match either one expression or another. This provides flexibility in specifying alternatives within a regex. We do not need to include this because in our bracket expressions, we already verify between capital and lowercase. 

### Flags

Regex flags are additional parameters that can be added to a regular expression to modify how the pattern matching is performed. These flags control various aspects of the regex matching process. Flags like i for case-insensitivity and g for global search modify how regex patterns are applied, altering the behavior of the regex engine. This is an email address only and not a password, meanng a flag is not needed. 

### Character Escapes

 
Regex character escapes are special sequences that represent characters with special meanings in regular expressions. They are used to match specific characters or character types in a regex pattern. Character escapes \ allow special characters to be used literally or give special meaning to characters that would otherwise be interpreted differently.We use this a few times in our code because it separates the different segments of the regex. 

## Author

This file was created by Destiny Jenkins, aspiring Software Engineer.
Github Repo: https://github.com/destinyjen/regex-tutorial
