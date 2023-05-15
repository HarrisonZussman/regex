# regex

A regex, or a regular expression, is a specific sequence of characters that specifies a search pattern in text. The most commonly used search patterns are string-searching or algorithms that find operations in strings which is used in input validation. Regex techniques were developed in theoretical computer science and formal language theory. When you see regex it help to look for common ground to recognize it for example (/^(-----+)@([\d-------]+).([-----]{---})$/.)

## Summary

The regex I will be covering is one that matches majority of email addresses. When validating emails, a good practice, which can almost be sure that a user will match the regex, is to limit what characters can input. The best way to guide the user into the regex method is by making them input something like 'gmail.com', 'yahoo.com', or 'xfinity.com' at the end of there email addresses.

## Table of Contents

- [regex](#regex)
  - [Summary](#summary)
  - [Table of Contents](#table-of-contents)
  - [Regex Components](#regex-components)
    - [Anchors](#anchors)
    - [Quantifiers](#quantifiers)
    - [Grouping Constructs](#grouping-constructs)
    - [Bracket Expressions](#bracket-expressions)
    - [Character Classes](#character-classes)
    - [The OR Operator](#the-or-operator)
    - [Flags](#flags)
    - [Character Escapes](#character-escapes)
  - [Author](#author)

## Regex Components
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` let break it down into segments to understand it.

Part 1 ([a-z0-9_\.-]+) this means that this part of the segment will have either a (a-z) lower or (A-Z) upper case letter a number from 0-9 and allow (_/.-) special character. The (+) means you can have infinite amount of characters

Part 2 ([\da-z\.-]+)  Validates the domain address for the email is valid.

Part 3 ([a-z\.]{2,6}) confirms that the email address extension is valid. The most common ones are .org, .gov, .com and .net. The international email addresses can end with .ca and .uk for an example

### Anchors

The anchors used in an email address validation regex are the ^ and $. (^) start it and ($) ends it.

### Quantifiers

At the end of the regex where it say {2,6} means the characters is between 2 and 6. That allows .com and .uk to work but .c and .abcdefghijklmnpoqrstuvwxyz not to work

### Grouping Constructs

Grouping can be used if needed to isolate a part of the string and to a back reference or to replace part of a string. 

### Bracket Expressions

Bracket expressions are used to define which characters will be matched within a regex. An example from the regex being used in this email regex is below. ([a-zA-Z.]{2,6})$/

### Character Classes

(\d) character class matches with a single character.

### The OR Operator

It will match the expression on regex before or after the / and can be used within a group or for an entire expression to help the computer understand the beginning and the ending

### Flags

For advanced searched flags are used. For an example after the (/) is (^) and before the (/) is ($). It is used to encase the expression without breaking it across multiple lines.

### Character Escapes

In a regex you will see a backslash that precedes a literal character. Examples are \w or \s.

## Author

Just a Web Devleopment Coding Boot Camp student
Github: https://github.com/HarrisonZussman/regex

