# Regex Breakdown

Introductory paragraph (replace this with your text)

 Symbols and letters are called characters and we use Regular Expressions for writing patterns to match and/or identify a specific sequence of characters or (in our case string). Regular Expressions are useful in taking out information from code. We use Regular Expressions to validate input or find/replace characters within a string.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

This tutorial will explain the use of Regex to match/verify emails. We will use the expression `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`. The email we will use in this is douglassnoddyjr@gmail.com. After defining the components there will be a link displaying my Regex, but you can also come up with your own!



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
Anchors are used to check if the mactching symbol  is the starter symbol or ending symbol of the input string. There are two types of anchors: the caret `^` and the `$`. `^` means the beginning of the string and `$` means the end of a string.
<br>

Test your own Regular Expression using `^` here<br>
https://regex101.com/r/cFJaGM/1 <br>

Test your own Regular Expression using `$` here<br>
https://regex101.com/r/toK1FT/1


### Quantifiers
Quantifiers specify how many occurences of a character group, or character class must be within the string. In this tutorial we will use the `+` operator, which will connect the `user email` to `email service` to `.com`. Another quantifier we are using here is `{2,7}`, which allows a range of 2-7 characters for the `email service` before the `.` in the email.
<br>

Test your own Regular Expression using `+` and `{integer,integer}` here<br>
https://regex101.com/r/eWWppM/1



### OR Operator

### Character Classes

### Flags

### Grouping and Capturing
Capturing groups are a way to treat multiple characters as a single unit. To group and capture we use the `()`. For example the Regular Expression `cat` creates a single group with the letters `"c" "a" "t"`. In this case for the tutorial the first capturing  group in this expression is `([a-z0-9_\.-])`, which is also the `user email`. The second capturing group is `([\da-z\.-]+)` which is the `email service`. The last capturing group is `([a-z\.]{2,7})` which is the `.com|net|org`.
<br>

Test your own Regular Expression using `()` here <br>
https://regex101.com/r/QKmRYM/1

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
