# regex

A regex, or a regular expression, is a specific sequence of characters that specifies a search pattern in text. The most commonly used search patterns are string-searching or algorithms that find operations in strings which is used in input validation. Regex techniques were developed in theoretical computer science and formal language theory. When you see regex it help to look for common ground to recognize it for example (/^(-----+)@([/-------]+).([-----]{---})$/.)

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

([a-z0-9_\.-]+) this means that this part of the segment will have either a (a-z) lower or (A-Z) upper case letter a number from 0-9 and allow (_/.-) special character. The (+) means you can have infinite amount of characters

([\da-z\.-]+) (\d) character class matches with a single character

### Anchors

### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
