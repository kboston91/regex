# Title (replace with your title)

This gist will serve as a walkthrough of the definition and use of regular expressions, also known as Regex. Regex is commonly used to filter and match pieces of data. Regex can be extremely complicated, but this tutorial will focus more on high level explanations. 

## Summary

The Regex I will be going over today is Matching an Email. This code can be used to make sure any input email follows the standard rules of all email format. 

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

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
The definition of an anchor is the beginning and end of an expression. If we are using the email code below, the anchors would be ^ and $.
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
### Quantifiers
Quantifiers exist to define the number of times a character must appear in the code. In the email code below, the quantifier is +, meaning it must contain at least one from the following list of characters a-z 0-9 . _-.
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
### OR Operator
the | in regex is used as an OR operator. Two different codes appear on either side of this symbol letting the user define the input as either the first code or the second code. 

### Character Classes
In the email code, the d allows the developer to place restrictions on the first character following the @ symbol. By adding \da-z, the developer is telling the user that the first character following the @ symbol must be a letter of the alphabet. 
### Flags
A flag is defined as follows: Flags, in a regular expression, are tokens that modify its behavior of searching
### Grouping and Capturing
In the email code below, the first grouping is ([a-z0-9_\.-]+)  The second grouping is ([\da-z\.-]+) and the third grouping is ([a-z\.]{2,6}). Grouping makes the user comply to each set of code before moving on to the next group. 
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
### Bracket Expressions
The content inside the brackets defines the characters allowed to be used.
### Greedy and Lazy Match
Greedy quantifiers are designed to match the longest possible string, so it keeps going. The lazy quantifier is designed to match the shortest possible string, so it is quicker.
### Boundaries
Boundaries would be used in a string to find specific words.
### Back-references
A backreference in a regular expression identifies a previously matched group and looks for exactly the same text again. 
### Look-ahead and Look-behind
This is used to match a specific order. 
## Author
Kourtney (suzette) Boston
https://github.com/kboston91/

Novice coder with limited experience. 

