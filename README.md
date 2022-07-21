# Regex-Tutorial

Within the following gist, an explanation for the components of a regular expression used to match a URL. 

## Summary


The regular expression of focus for this tutorial is the regular expression to match a URL /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
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
Anchors are used to match the beginning and end of the string postion. The anchor for the beginning of the string used in the example is the "^" right before the first capturing group, which denotes the beginning of the single string and the anchor "$" is used to denote the end of the string being matched.

### Quantifiers
The quantifier is used to determine how a character or characters is matched. For example the question mark at the end of the "(https?:\/\/)?" capturing group is looking for the match of https:// or nothing. In this case, there will be a match if there is either nothing in place of the first capturing group or if the exact string https:// is there. Anything in between or more than 1 instance of it will not match.
### OR Operator

### Character Classes
Character classes give the exact or range of characters needed to make a match. In the example chosen, "a-z" references the capturing group must contain letters from lowercase a to z to create a match. Another character class is the "\d" used in the second capturing group which is the character class of digit, which matches with any digit character(0-9).
### Flags

### Grouping and Capturing
The capturing group is a bound group of tokens used to extract a substring or use as a back reference. These capture groups are surrounded by parens such as 
"(https?:\/\/)" within the example.
### Bracket Expressions
Bracket expressions are used to match the specific quantity of the token/grouping it follows. In the example, the "{2,6}" bracket expression is looking for the quantity of tokens within the boundaries of "[a-z\.]" to be 2 to 6 tokens to be a match.
### Greedy and Lazy Match
A greedy match refers to the "*" symbol used in the example. When noted, it looks for as many matches of the characters as possible. It doesnt have a lower or upper limit of how much it is looking for, but is defined by what it is following. For example the "[\/\w \.-]*" capturing group is looking for a backslash followed by any word character, will match with 0 instances or as many instances as it can find.
### Boundaries

### Back-references

### Look-ahead and Look-behind

### Escaped Characters
escaped characters are notated starting the the "\" followed by the literal special or unicode character that must be matched. In the example "\." is denoting that at that section in the string, a literal "." must be found for there to be a match. Using escaped characters is used within the first capturing group "(https?:\/\/)" which is looking for two "//" symbols after the https or there will not be a match.

## Author
I am a full stack web development student.
Find me at Github under [samb56](https://github.com/samb56)
