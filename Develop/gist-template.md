# Title (replace with your title)

Welcome to this beginner-friendly guide on regular expressions, or regex for short. Regex can seem tricky at first, but it's just a way to find specific patterns in text, like looking for certain words in a book. In this tutorial, we'll explore a simple regex together, showing you how these patterns work and how they can be really useful in your coding journey.

## Summary

We're gonna be analyzing a regex which is used to validate email addresses: 

/^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}$/

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
Anchors indciate where the regex pattern starts and ends. In this pattern:
'^' is showing the start of the line of code
'$' means end of the line 

### Quantifiers

'+' means one or more of the previous character class. So, '[a-zA-Z0-9._-]+' means one or more of any letter, number, dot, underscore, or hyphen.

### OR Operator

The OR Operator lets the regex pattern choose between alternatives, and this is incidatced by this: '|' . In this specific regex, there is no explicit OR operator.

### Character Classes
'a-zA-Z0-9._-' : This is the first part. It matches uppercase and lowercase letters, numbers, dotes,underscores, and hyphens.
'a-zA-Z0-9.-' This is the second part. It accomplished the same thing as the first part but without the underscore.
'@' is a character that matches itself. We see this character in all email addresses.

### Flags

Flags are usually at the end of the regex to change its behavior. For example, 'g' stands for 'global search'. However, this regex pattern doesn't contain any flags. 

### Grouping and Capturing

This specific regex pattern does not use grouing and capturing mechanisms. However, many do, often with something like a paranthesis. If a part of the regex is inside a paranthesis, those characters are being grouped together. The characters inside the paranthesis that make up that group will be matched to similar strings of characters. Capturing occurs when the group in a regex captures the contgent it matches. You can assign one group with the number 1, and another with the number two. Then you can refer back to the captured content with numbers 1 and 2. 

### Bracket Expressions

The bracket expressions are '[a-zA-Z0-9._-] and [a-zA-Z0-9.-]'. They define a group of characters to match and let the regex pattern match Character classes referenced earlier.

### Greedy and Lazy Match
Greedy and lazy matching are about how much the regex retrieves from the text. Either it will take as much as possible (greedy) or as little as possible (lazy). Bascially, this lets us know how much the regex pattern is trying to match. 

### Boundaries

Boundaries are not used in this regex pattern, however, they are useful for making sure pattens occur at specific parts of the pattern. They look like '\b'

### Back-references

Back references look like '\1', '\2', and it's used to match the same characters that were matched by a capturing group. Back references are not used in this regex pattern. 

### Look-ahead and Look-behind

This feature is not part of the regex pattern. Look-ahead and look-behind allow the regex pattern to exclude or include patterns based on what precedes or follows a point in the pattern. 

## Author
I'm a student at a full-stack coding bootcamp. You can visit my github profile at https://github.com/Artemis051


