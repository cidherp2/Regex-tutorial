# Regex tutorial E-mail validation

As web developers is really important to handle account creation in a correct manner, and this includes validating that the e-mails given by the user are formatted correctly, to ensure the correct functionality of our web apps.

## Summary

the regex that'll be used is the following one:
 /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
This expression helps us validate, that the user is writing a valid e mail, this tutotial will explain how each part of the regex works and what it means so yo can use it in your code if necessary.


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
The anchors for this regex are the following
 ^ This anchor shows is the start of the expression
 $ This anchor shows us that it is the end of the expression 

### Quantifiers
Quantifiers specify how many times the previous character or group should be matched
' + ' Matches the preceding items one or more times, in this case defines that the next part is part of the regex
' {2,6} Matches the preceding item between 2 and 6 times.

### OR Operator
The || or operator isnt present in this regex.
### Character Classes
A character class is a set of characters that can match any character in the input string given, in this particular regex we have 3 character classes

[a-z0-9_\.-]+) @ - The username in the email, the class tells it it's a string that can contain any lower case character from a to z any digit from 0 to 9, underscore, dot or hyphen. It must contain an '@' after 

[\da-z\.-]+ /. -This is for the domain and it goes after the @ it validates that this string contains any digit, any lowercase letter, dot or hyphen. it also validates that is followed by a single dot

[a-z\.]{2,6} Matches any lowercase letter or dot that appears between 2 to 6 times.

### Flags

### Grouping and Capturing
We group through expressions and through parentheses in this case we group wit +) @ after the username and +). after the domain example ".com" 
### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
