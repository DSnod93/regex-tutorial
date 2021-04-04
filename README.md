# Email Match: Regex Tutorial

# <b> Regex Breakdown </b>

 Symbols and letters are called characters and we use Regular Expressions for writing patterns to match and/or identify a specific sequence of characters or (in our case string). Regular Expressions are useful in taking out information from code. We use Regular Expressions to validate input or find/replace characters within a string.

## Summary

This tutorial will explain the use of Regex to match/verify emails. We will use the expression `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`. The email we will use in this is douglassnoddyjr@gmail.com. After defining the components there will be a link displaying my Regex, but you can also come up with your own!



## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## <b> Regex Components </b>

### <u> Anchors </u> 
Anchors are used to check if the mactching symbol  is the starter symbol or ending symbol of the input string. There are two types of anchors: the caret `^` and the `$`. `^` means the beginning of the string and `$` means the end of a string.
<br>

Test your own Regular Expression using `^` here<br>
https://regex101.com/r/cFJaGM/1 <br>

Test your own Regular Expression using `$` here<br>
https://regex101.com/r/toK1FT/1


### <u> Quantifiers </u>
Quantifiers specify how many occurences of a character group, or character class must be within the string. In this tutorial we will use the `+` operator, which will connect the `user email` to `email service` to `.com`. Another quantifier we are using here is `{2,7}`, which allows a range of 2-7 characters for the `email service` before the `"."` in the email.
<br>

Test your own Regular Expression using `+` and `{integer,integer}` here<br>
https://regex101.com/r/eWWppM/1

### <u> Character Classes </u>
The character class used in this tutorial is `\d` which matches a digit 0-9.

### <u> Grouping and Capturing </u>
Capturing groups are a way to treat multiple characters as a single unit. To group and capture we use the `()`. For example the Regular Expression `cat` creates a single group with the letters `"c" "a" "t"`. In this case for the tutorial the first capturing  group in this expression is `([a-z0-9_\.-])`, which is also the `user email`. The second capturing group is `([\da-z\.-]+)` which is the `email service`. The last capturing group is `([a-z\.]{2,7})` which is the `.com|net|org`.
<br>

Test your own Regular Expression using `()` here <br>
https://regex101.com/r/QKmRYM/1

### <u> Bracket Expressions </u>
Bracket Expressions `[]` or `()` group part of the regular expression together. For this tutorial we have brackets for the first set of characters `[a-z0-9_\.-]`, which matches any letter a-z and any number between 0-9. In addition, it matches the special characters `_` and `-`. The second set of characters `[\da-z\.-]` matches a single digit from 0-9 and any character a-z and special characters `.` and `-`. Lastly, character set `[a-z\.]` matches any character a-z and the character `"."` . 
<br>

Test your own Regular Expression using `[]` or `()` here <br>
https://regex101.com/r/mgy8sJ/1

### <u> Greedy and Lazy Match </u> 
This tutorial includes Greedy matches meaning the expression will match as large a group as possible. In addition, since we are using the `+` Quantifier it will match as many times as needed. `{}` is also another7 Greedy Quantifier since we are including the matches between both `{2,7}`.
<br>

## Author 
<hr>

You can view my work at https://github.com/DSnod93


