# Your guide to the basics of Regular Expressions

Introductory paragraph (replace this with your text)

## Summary

The regex expression that I will be going over today is /^(?=.*[A-Za-z])(?=.*\d)(?=.*[@$!%*#?&])[A-Za-z\d@$!%*#?&]{8,16}$?.  This regex expression can be used to make sure that a string has at least one uppercase, lowercase, number, and special character in it.  You would probably use this to make sure a user has submitted a strong enough password.  We will be going over each individual component of this expression to make sure you understand how it all works together. 

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

The anchors in a regex start and end the expression.  The ^ begins an regex expression.  The information following the ^ must be included at the start of the expression. ^Must would mean that the string must start with "Must" and this is case sensitive.  The $ at the end of a regex expression means that the string must end with whatever precedes the $.  So end$ would mean that the string must end with "end". 

### Quantifiers

Quantifies are used to set what the limits of your regex will accept.  For example in our regex the * is saying the preceding information zero or more times.  They are greedy which means that they search the whole expression for as many examples of the * as possible.  

### OR Operator

The OR operator | is used to check whether one of multiple things is present.  (a|z) will check if the string has either an a or a z.  

### Character Classes

Character classes are an easy way to define a group of characters quickly.  The . class matches any character that isn't a new line operator. The \d class that looks for a alphanumeric digit is a faster way of saying [0-9]. 

### Flags

Flags are used after the end of the regex expression to add additional search information.  The g flag means the regex should be used against all possible matches in a string.  The i flag is used to ignore case sensitivity in a search.  

### Grouping and Capturing

Grouping and capturing can be used to number matches so that they can be back refrenced.  Withing parens (abc) captures all the matches of "abc".  So the string "abcabcabc" will have 3 matches that can be backrefrenced with numbers that represent the order they were found in. 

### Bracket Expressions

Bracket expressions are used to capture a range of allowed characters.  [a-z] can be used so search for all lowercase letters between and including a-z. 

### Greedy and Lazy Match

Greedy expressions are used to search for all possible matches of an expression and lazy 

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
