# Using Regex to Validate Emails

What is a (Regex) Regular Expression? 

A Regular Expression(Regex)is a pattern or filter that describes a set of strings that matches the pattern.

## Summary


In our [Regex Example](#regex-example) we will break down the parts as they relate to testing or validating emails as strings. It simply checks for the presence of a number, letter, or a special character (underscore, period, or hyphen) in its first section. The second section is followed by an "@" symbol, then one or more alphanumeric characters or special characters followed by a period. The third section then filters for two to six alphanumeric characters. 

This allows developers to account for multitude of alphanumeric combinations and still confirm the expected result.

```json
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```

If all of these components are present, the string is considered a valid email address.

## Table of Contents

- [Regex Example](#Regex-Example)
- [Regex Components Defined](#quantifiers)
- [Position Anchors](#position-anchors)
- [Grouping/Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)
---

# Regex Example:
The following regex code is being used to validate email addresses: 
```json
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
### The three sections are broken down as follows:

The first section, ```[a-z0-9_\.-]+``` specifies that one or more alphanumeric characters, underscores, periods, or hyphens must be present. This is followed by the @ symbol that exists in all email addresses.

The second section, ```([\da-z\.-]+)``` specifies that one or more digits, lowercase letters, periods, or hyphens must be present.

The third section, ```([a-z\.]{2,6})``` specifies that two to six alphanumeric characters or periods must be present.

---

## Position Anchors

## Quantifiers

## Grouping/Capturing

## Bracket Expressions

## Character Classes

## The OR Operator

## Flags
A flag is an optional parameter to a regex that modifies its behavior of searching. A flag changes the default searching behavior of a regular expression. It makes a regex search in a different way. A flag is denoted using a single lowercase alphabetic character.

## Character Escapes
The \ is known as the escape code, which restore the original literal meaning of the following character. Similarly, * , + , ? (occurrence indicators), ^ , $ (position anchors) have special meaning in regex. You need to use an escape code to match with these characters.

---
## Author:
---
John Lopez is a student of full stack web development. 

You can follow the link to the author's GitHub profile ---> [Author's Profile](https://github.com/Think-Again-Coder) where you will find other projects. 
