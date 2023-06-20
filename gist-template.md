# Matching a Hex Value with RegEx



## Summary

In this gist I will be disecting a hex value using regEx or regular expressions. The hex value I will be using in this example is '/^#?([a-f0-9]|[a-f0-9{3}])$/'.

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
Anchors are used to match a position before, after, or between characters.
- "^" matches the beginning of the text string
- "$" matches the end of the text string

In the hex value provided you can see the '/^#?([a-f0-9]|[a-f0-9{3}])$/' everything in between the carrot and money sign will be searched for with regex.

### Quantifiers
Quantifiers specify how many instances of a character or group of characters must be present in the in puts for a match to be found.
-* matches 0 or more times
-+ matches 1 or more times
-? matches 0 or 1 time
-{n} matches exactly n times
-{n,} matches at least n times
-{n,m} matches from n to m times

In the hex value provided '?([a-f0-9]|[a-f0-9{3}])$/' represents that after the # 0 or 1 characters will be present.'{3}])$/' 

### Grouping Constructs
Grouping contructs let you extract a subset of information from a token of text, they also can be used to isolate a part of a string.

-(espr) matches or captures the group in the parenthesis

In the example we are disecting '([a-f0-9]|[a-f0-9{3}])' you can see we are targeting one the the subsets in the or statement depending on the input.

### Bracket Expressions
Bracket expressions indicate a set of characters to match with the input.

In the hex value provided '[a-f0-9]' and '[a-f0-9{3}]' are both examples. In the first example we are searching for two strings that match a-f and 0-9.

### Character Classes
Character classes are a set of characters enclosed in square brackets that allow for more compact RegEx.

-/d one digit characters 0-9
-/w word characters (Unicode letter, digit, or underscore)
-/s white space characters

There are no examples of this in the hex value we are evaluting.

### The OR Operator
The OR operator impliments the logical or operation.

In the hex value we see this in '[a-f0-9]|[a-f0-9{3}]' the operation a-f0-9 will be performed OR a-f0-9{3} will be performed.

### Flags
Flags allow for functionality in searching.

-g global search
-d substring matches
-i case insensitive search

There are no examples of this in the hex value we are evaluating.
### Character Escapes

## Author

A junior developer in training at George Washington University.
https://github.com/ashleytrollinger
