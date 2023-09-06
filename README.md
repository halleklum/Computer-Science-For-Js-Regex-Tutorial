# Regex Tutorial: Email
Within this tutorial, I am going to explain how regex is used to match emails. This allows users to validate the structure of an email address and can be changed to allow for different variations. 

## Summary
Regular expressions define a search pattern with a specific sequence of characters. Within this article I am going to break down the different parts of a regex, look at what each part does, and apply what I learned to an example. The expression I will use for the example will be `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` .
  
## Table of Contents:
1. [Anchors](#Anchors) 
2. [Quantifiers](#Quantifiers)
3. [Character Classes](#CharacterClasses)  
4. [Grouping and Capturing](#GroupingAndCapturing)
5. [Bracket Expressions](#BracketExpressions)
6. [Greedy and Lazy Match](#GreedyAndLazyMatch)
7. [Author](#Author)

## Regex Components

### Anchors
In this example, the anchors used for matching an email are `^` and `$`. The beginning of a string will be indicated by `^` and the end of the string is indicated by `$` .
  
### Quantifiers:
In this example, the quantifiers includes `+` and `{}`. The `+` will connect the users email, name, email service, and the `.com` . The `{2,6}` sets a parameter of 2-6 characters for the set of `[a-z\.]` .
  
### Character Classes:
In this example, the character class is `\d` . This matches any digit between 0-9.
  
### Grouping and Capturing:
Within this example, there are 3 groups present. The first group is `([a-z0-9_\.-]+)` which defines the users email name. The second group is `([\da-z\.-]+)` which defines the email service or domain name. The last group is `([a-z\.]{2,6})` which is used to capture the domain extension such as `.com` or `.net`.
  
### Bracket Expressions:
Within this example, there are 3 bracket expressions. The first is `[a-z0-9_\.-]` which is matching the case sensitive letters a-z, digits 0-9, and the characters `_`, `-` , `.`. The second bracket expression is `[\da-z\.-]` which is matching the case sensitive letters a-z, any digit between 0-9, and `.` , `-`. The third bracket expression is `[a-z\.]` which matches case sensitive letters a-z and `.` .
  
### Greedy and Lazy Match:
In this example, there are two greedy quantifiers; `+` and `{}` . These will let the match expand as long as it has to. For learning purposes, if the quantifiers were lazy, they would set the system to complete the shortest match. 
  
## Author
Hello! My name is Halle Klum and you can view my other projects at https://github.com/halleklum . 
    


