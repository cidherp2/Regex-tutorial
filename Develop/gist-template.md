# Regex tutorial E-mail validation

As web developers, it is crucial to handle account creation correctly, including validating user-provided emails to ensure the proper functionality of our web apps.

## Summary

The regex used for email validation is:

### regex
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

###

This tutorial will explain each part of the regex and its meaning so you can use it in your code if necessary.

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
- [Author](#author)

## Regex Components

### Anchors
The anchors for this regex are:
- `^`: Start of the expression
- `$`: End of the expression

### Quantifiers
Quantifiers specify how many times the previous character or group should be matched.
- `+`: Matches the preceding items one or more times.
- `{2,6}`: Matches the preceding item between 2 and 6 times.

### OR Operator
The OR operator (`||`) isn't present in this regex.

### Character Classes
A character class is a set of characters that can match any character in the input string. This regex has 3 character classes:
1. `[a-z0-9_\.-]+)@`: Username in the email, allowing lowercase letters, digits, underscores, dots, or hyphens.
2. `[\da-z\.-]+`: Domain after the '@', allowing digits, lowercase letters, dots, or hyphens. It must be followed by a single dot.
3. `[a-z\.]{2,6}`: Matches lowercase letters or dots in the TLD between 2 and 6 times.

### Flags
No flags are used in this regex.

### Grouping and Capturing
Grouping is done with parentheses `()`. In this regex, two main groups capture:
1. `([a-z0-9_\.-]+)`: Username
2. `([\da-z\.-]+)`: Domain
3. `([a-z\.]{2,6})`: TLD

These captured groups can be useful for extracting specific parts of the email.

### Bracket Expressions
Bracket expressions define sets of characters. In this regex:
- `[a-z0-9_\.-]`: Matches lowercase letters, digits, underscores, dots, or hyphens in the username.
- `[\da-z\.-]`: Matches digits, lowercase letters, dots, or hyphens in the domain.

### Greedy and Lazy Match
The quantifiers in this regex (`+` and `{2,6}`) are greedy, matching as much as possible.

### Boundaries
The `^` and `$` anchors ensure the regex matches the entire string.

### Back-references
No back-references are used in this regex.

### Look-ahead and Look-behind
Look-ahead (`(?=...)`) and look-behind (`(?<=...)`) assertions are not present in this regex.

## Author

 Written by  Alejandro Larios, Reach out on my github profile [cidherp2](https://github.com/cidherp2) for more exciting projects and contributions!
