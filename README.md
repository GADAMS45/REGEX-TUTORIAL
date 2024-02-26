# Regex Tutorial For Matching An Email

Welcome to the world of Regular expressions--REGEX for short. Regex are powerful tools that make programming and text processing easier. In this tutorial we will explore the many different parts of Regular expressions.

## Summary

In this tutorial we will go over  ```/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/```.  This regex code is used to match and validate emails and their format.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

This regex expressions contains a couple of anchors -- ```^```and `$`.  ```^```Indicates the beginning of expressions and `$` symoblizes the end of the expression. 

### View them in the code below
```regex
 /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
 ```

### Quantifiers

Quanitfiers connect parts of the code in the string.  For exmple this code uses ```+``` that is an opertor which connects emailname, email servicer and the .com ending.  this code also includes ```{}``` which churly brackets are known for rane identifiers which can be seen at the end of the expression below. ```{2,6}```sets the range of numbers for the ending of the email in this set ```[a-z\.]```.  This is saying for the ".com" portion of the email it can have any letters in there (no numbers) but gives a range from 2 charecters to 6.  for example you've seen: .co,.uk, .ca or .com.

### View them in the code below
```regex
 /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
 ```

### Character Classes


```\d```is one of the most basic regex character class that will return and any digit from 0-9.  You can also see them as the total enclosed in asquare brackets ```[]```.


### View them in the code below
```regex
 /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
 ```



### Grouping and Capturing

Grouping and Caputuring in regex is defined by code placed between two square baracket ```()``.  This regex code has three groupings.  One is the email name ([a-z0-9_\.-]+) , Two is the email servicer name ([\da-z\.-]+)\ and three is the .com name at the end ([a-z\.]{2,6}).

### View them in the code below
```regex
 /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
 ```



### Bracket Expressions
THis line of code has three bracketed expressions that correlate to each part of an email address.

[a-z0-9_\.-] This expression matches the username and allows it to have any letters and numbers 0-9.  It also allows additional charecters such as an underscore "_", Perios ".", and a dash "-".

[\da-z\.-]  This expression is for the domain name and allows you to match any digit, letters and additional charaters period "." and dash "-".

[a-z\.]{2,6}  Last but not least is the .com code which allows you to match any letter and in the length from 2  characters to 6.

### Greedy and Lazy Match



### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

This was written by Greg Adams a Firefighter Paramedic trying to be a coder. Check out some of my work here at: https://github.com/GADAMS45