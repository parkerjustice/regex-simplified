# Regex Simplified

Regex Simplified is a quick and easy tutorial that explpains what regex (regular expressions) are and their uses. After this tutorial you should find that this is a simple way of learning a daunting new challenge.

## Summary

In this tutorial I will be going over what goes into regular expressions and how they are used. Regex is a sequence of patterns that are use to replace characters in strings. These strings and patterns are used for many different things such as URLs, HTML, Email, or even Hex Values. These help create a unique place for specific links to occure. Here is a good example of what a regex is:

# URL regex
` /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

We will go further into what regex is and all the details along this tutorial.
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

`/^`(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?`$/`
We need to start from the beginning, which would be anchors. Anchors are what the expression has at the beginning and the end that are highlighted. The `^` Matches the beginning of the string while the `$` Matches the end of the string. They are used to signify the beginning or the end of an expression.

### Quantifiers
 /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

 We will now be going over quantifiers and what they do. A quantifier was used to show how many of the characters are to be expected. This means it shows how often a character, class, or character group would need to be available in the input for any sort of match to become usable. Quantifiers is what we like to call greedy and will match to just about anything they van that is why you need to pay attention to them. 

Here are a few examples of what is being explained:

+ matches one or more preceding tokens
{2,6} this one will match two to six of the previous token

### OR Operator
Hex Expression
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

The `|`repressents the "or". The "or" is the operator and is shown as using the `|` character. This matches the expression that comes before or after it.

### Character Classes
Character classes are used to match a specific character to a set.
A few examles are as follows:

[A-Z] This shows a "range" of characters and giving the person knowlege that you are able to use every letter between them. 
.This will accept any input and is a great use if you are in a pinch
\p This matches a character with unicode.

There are lots of other examples that we could add but would take up too much time. A simple google search or link would give you every character class. 
### Flags

Flags are a great way of changing how an expression is understood. A flag forces regex to search things in a different way and is always shown to use a single lowercase letter such as these:
| Letters   | Meaning       | 
| ------------- |:-------------:| 
| i    | makes an expression case-insensitive |
| g   | makes an expression search for all occurrences     |   
| s | makes the character . match newlines      |    


### Bracket Expressions
 /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

 A bracket expression [] matches a character set that is inside the two brackets. This is shown with this example with a-z being within the two brackets a character will be matched within that example. Another example that is not mentioned would be [0-9] because it also works numerically as well. 
 Regex will match any single characger together, go back to the character class tag to learn more.

## Author

Parker Justice is an aspiring developer with a love for front-end developing. 
