# Matching an Email with Regex

 A regex is short for regular expression. It's a simple way to search for a pattern within an input. In this example i'll be using an Email Regex that validates a matching email. 

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

To begin, a regular expression looks something like this `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`. It's letters and numbers divided into sections to dictate validation. In this tutorial I will break apart this code and thoruougly explain each section.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Flags](#flags)

## Regex Components

### Anchors

The anchors in this regex can be seen at the beginning and the end of a string. The first one is `^` and the last one ends with a `$` symbol.

### Quantifiers

The quantifiers are used to form complex regular expressions. Quantifiers can be something like the `+` sign. In the email validation, the `+`, and the `{2,6}` are used for different purposes. The `+` sign is used to connect the users email name, service and `.com`. The `{2,6}` are used to match characters between 2 and 6.

### Bracket Expressions

Bracket Expressions are what holds the code together and divides it by sections. For example, the first one is `[a-z0-9_\.-]` and it searches the alphabet from a through z or a number from 0-9. The the regex uses quantifiers to put the code together.



### Character Classes

This is a fairly simple one as it only tries to match one thing. The `\d` character class is used to match a single number from 0-9. It doesn't not match any two numbers like 22. 


### Flags

Regular expressions have optional flags that allow for functionality like global searching and case-insensitive searching. These flags can be used separately or together in any order, and are included as part of the regular expression.

In our case we arn't using any flags, but if we were it would be at the end. For example, `([a-z\.]{2,6})$/g`. This `g` at the end indicates a global search that will match all occurrences. Without the `g` it'll only text for the first one. 


## Author

My name is Christian Nunez and I am a Full Stack Web Developer.
Github Profile: https://github.com/chrisnunez