# REGEX-Tutorial: Matching an Email

In this challenge, users will become acquainted with Regular Expressions, commonly known as regex. Regular Expressions consist of a sequence of special characters that define a search pattern within text.

## Summary

    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

In this lesson, we will delve into the example regex provided above. What might initially appear as a random combination of characters is, in fact, the subject of our tutorial that aims to enhance your understanding. Each of these characters plays a specific role in how regular expressions operate. By the end of this tutorial, you will gain a comprehensive understanding of the components involved in analyzing this email pattern.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)

## Regex Components
Since the regex is a literal, it must be wrapped in slash characters  // . This is explains their presence at the front and end of the string. 

### Anchors
    ^ : Anchors the pattern at the beginning of the string
    $ : Anchors the pattern at the end of the string
### Quantifiers
    + : Matches one or more of the preceding token
### Character Classes
    [a-z0-9_\.-] : Matches any lowercase letter, number, underscore, dot(.), or hyphen
### Grouping and Capturing
    (....) : Parentheses represent grouping and capturing. 
        ([a-z0-9_\.-]+) : captures the username part
        ([\da-z\.-]+) : captures the domain name
        ([a-z\.]{2,6}) : captures the Top-Level 
        domain(TLD). For example: .com, .org
### Bracket Expressions
    [a-z0-9_\.-] : represents a character class that matches any of the characters inside of the brackets
### Greedy and Lazy Match
    Outside of + which are greedy by default, there isn't a case of lazy in this expression
### Boundaries
    ^ and $ act as boundaries that ensure the entire string match the pattern
## Author
I'm DeAngelo and am working towards becoming a fullstack developer. If interested, here is a link to view my work in Github: https://github.com/dtjones23