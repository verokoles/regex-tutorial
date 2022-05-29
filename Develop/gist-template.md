# REGEX TUTORIAL
## User-Story
"AS A web development student <br>
I WANT a tutorial explaining a specific regex <br>
SO THAT I can understand the search pattern the regex defines."
<br>
<br>
In this template, a tutorial is given on regex (Regular Expressions), <br>
 a series of special characters that define a search pattern. <br>


## Summary

I will be going over the expression on how to validate a user's email address. <br>
code snippet: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
## Table of Contents

- [REGEX TUTORIAL](#regex-tutorial)
  - [User-Story](#user-story)
  - [Summary](#summary)
  - [Table of Contents](#table-of-contents)
  - [Regex Components:puzzle:](#regex-componentspuzzle)
    - [Anchors:anchor:](#anchorsanchor)
    - [Quantifiers:plus_sign:](#quantifiersplus_sign)
    - [OR Operator](#or-operator)
    - [Character Classes](#character-classes)
    - [Flags:flag:](#flagsflag)
    - [Grouping and Capturing](#grouping-and-capturing)
    - [Bracket Expressions](#bracket-expressions)
    - [Greedy and Lazy Match](#greedy-and-lazy-match)
    - [Boundaries](#boundaries)
    - [Back-references](#back-references)
    - [Look-ahead and Look-behind](#look-ahead-and-look-behind)
  - [Author](#author)

## Regex Components:puzzle:
Regular Expressions are also considered literals, wrapping in special characters like slashes `/`.
### Anchors:anchor:
Anchors are the wrapping symbols which indicate the START and FINISH of the regular expression. <br>
 In the code snippet for validating a user's email address, the regex starts with the `^` and ends with the `$` symbol. <br>
These start and end points 
### Quantifiers:plus_sign:
The different quantifiers in this snippet include brackets, `{}` as well as the plus sign, `+`. <br>
Brackets 
### OR Operator
An example of an OR operator would be the `` symbol. These operators simply 
### Character Classes

### Flags:flag:

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match
These are quantifiers in  regex that basically shorten or elongate the string returned. <br>
The default behavior of these regexes are to be greedy, or to extract as long of a possible string version. <br> 
In this email verif snippet, the greedy match would come from the symbol `+` that appears after the first and second set of `[]`.
`^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$` <br>
Lazy, on the other hand, is simply the shortest possible string for the regex. <br>
 A lazy match could be `+?` or `*?` groupings, but in this regex we have none. <br> 
So this expression always returns the greatest possible string.
### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

 My name is Veronica Kolesnikov, a junior developer from San Antonio, TX.<br>
 Currently finishing a full-stack dev bootcamp and becoming employed in front-end and/or back-end.<br>

[:octocat: Github Profile](https://github.com/verokoles)
