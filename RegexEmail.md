# Email Regex gist

This is a gist to help people understand more about regex, and simaltainiusly help me learn by teaching others. In this gist we'll go over how the syntax of the regex operation works to find a value that mathches. We will learn about the diffrent componets of regex and how you can construct your own regular expression!

## Summary

I will be summarizing matching an email with the following regex expression ( `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` ) 

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

lets break down the regex into bite size pices

1) /^

2) ([a-z0-9_\.-]+)

3) @

4) ([\da-z\.-]+)

5) \.

6) ([a-z\.]{2,6})

7) $/

### Anchors

In this case 1 ( /^ ) and 7 ( $/ ) are anchors. Anchors are used to start and stop and declare the regex!

The / starts or ends the expression, think of it like parentheses in a math problem.

The ^ declares that the regex is a string

The $ signifies the end of the string 

So a regex of /^ $/ is a string 

### Quantifiers

In this case 2 ([a-z0-9_\.-]+) , 4 ([\da-z\.-]+) , and  6 ([a-z\.]{2,6}) have Quantifiers. Quantifiers just set  limits to regex operations.

The + is a limiter its telling this part of the expression it can have one or more matches to the pattern 

The {2,6} is a range of how many characters the part can have 

The () is a [Bracket Expressions](#bracket-expressions)

The [] is a [Bracket Expressions](#bracket-expressions)

The a-z or 0-9 are a [Bracket Expressions](#bracket-expressions)

The - is a [Bracket Expressions](#bracket-expressions)

The \d is a [Character Class](#character-classes)

The \. is a [Character Escape](#character-escapes)

So ([]{2-6}) is part of a regex that has only 2 to 6 characters

### Grouping Constructs

Grouping constructs are how you make complex things like a email! in thhis case 2 though 6 are Grouping Constructs. Grouping Constructs are used to to break up sections in complex regex operations!

The () (2 , 4 and 6) and everything in them is a [Bracket Expressions](#bracket-expressions) , but the whole thing is a grouping construct that come toether to make the one complex string

The @ and \. (5 is a [Character Escapes](#character-escapes) ) , can come toether to make the one complex string

so a ()@() in terms of regex is a complex string that is a like "cat@cat"

### Bracket Expressions

In this case 2 ([a-z0-9_\.-]+) , 4 ([\da-z\.-]+) , and  6 ([a-z\.]{2,6}) are Bracket Expressions. A Bracket Expression is use d to define what characters can accure in the parentheses! 

The () just act as a divider to signify this is a diffrent part of the string.

The [] just act as a list of characters that are approved for this part of the string.

The a-z or 0-9 are the list of characters that are aproved. 0-9 is ( 0 , 1 , 2 ,3 , 4 , 5 , 6 , 7 , 8 , 9 ) or zero through nine. Same with a-z its the entire alpabet, but onlu lower case upper case is A-Z

The - in 2 or 4 is litteraly just the - character 

The + is a [Quantifier](#quantifiers)

The \d is a [Character Class](#character-classes)

The \. is a [Character Escape](#character-escapes)

The {2,6} is a [Quantifier](#quantifiers)

So ([a-z]) is part of a regex that has all lower case characters 

### Character Classes

In this case 4 ([\da-z\.-]+) their is a Character Classes. A Character Class is used to define what charcaters can ocuur in the regex operation or [Grouping Constructs](#grouping-constructs)!

The \d is the same as the [Bracket Expressions](#bracket-expressions) 0-9 it lets you use any Arabic numeral digit.

The () is a [Bracket Expressions](#bracket-expressions)

The [] is a [Bracket Expressions](#bracket-expressions)

The a-z is a [Bracket Expressions](#bracket-expressions)

The - is a [Bracket Expressions](#bracket-expressions)

The \. is a [Character Escape](#character-escapes)

The {2,6} is a [Quantifier](#quantifiers)

The + is a [Quantifier](#quantifiers)

### The OR Operator

While not used in this email regex or operators are usfull. They can be used in a [Bracket Expressions](#bracket-expressions) to signify it can be this or this. in example we could say the string is only lower case letters or numbers ( a-z | 1-9 ). They are signaled by the pipes symbol ( | ).

### Flags

While not used in this email flags are usfull. They are kida weird thou they go outside the slashs that are in the expression and define addional funcionality or limits for the regex operation. For instince one can make the expression case insensitive!

### Character Escapes

In this case 2 ([a-z0-9_\.-]+) , 4 ([\da-z\.-]+) , 5 ( \. ), and  6 ([a-z\.]{2,6}) have Character Escapes. A Character Escape is used when a character could signal something in regex, but you need said character. It allows you to use characters by typeing a \ before the character you want

The \. means that a period is or can accure in this spot

The \d is a [Character Class](#character-classes)

The a-z or 0-9 are a [Bracket Expressions](#bracket-expressions)

The - is a [Bracket Expressions](#bracket-expressions)

The () is a [Bracket Expressions](#bracket-expressions)

The [] is a [Bracket Expressions](#bracket-expressions)

The + is a [Quantifier](#quantifiers)

The {2,6} is a [Quantifier](#quantifiers)

So ([a-z]) is part of a regex that has all lower case characters 

## Author

Im a new devolper trying to learn and help others my digital portfolio is here https://jbird11801.github.io/Portfolio/ and my profile is https://github.com/jbird11801!
