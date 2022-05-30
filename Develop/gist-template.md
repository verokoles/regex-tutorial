# REGEX TUTORIAL
## User-Story
"AS A web development student <br>
I WANT a tutorial explaining a specific regex <br>
SO THAT I can understand the search pattern the regex defines."
<br>
<br>
In this template, a tutorial is given on regex (Regular Expressions),
 _a series of special characters that define a search pattern_. <br>


## Summary

This template will be going over the expression on how to **validate a user's email address**. <br>
Code snippet: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
## Table of Contents

- [REGEX TUTORIAL](#regex-tutorial)
  - [User-Story](#user-story)
  - [Summary](#summary)
  - [Table of Contents](#table-of-contents)
  - [Regex Components:jigsaw:](#regex-componentsjigsaw)
    - [Anchors:anchor:](#anchorsanchor)
    - [Quantifiers:plus_sign:](#quantifiersplus_sign)
    - [OR Operator:``:](#or-operator)
    - [Character Classes:](#character-classes)
    - [Flags:triangular_flag_on_post:](#flagstriangular_flag_on_post)
    - [Grouping and Capturing:paperclips:](#grouping-and-capturingpaperclips)
    - [Bracket Expressions []](#bracket-expressions-)
    - [:heavy_plus_sign:Greedy and Lazy Match:heavy_minus_sign:](#heavy_plus_signgreedy-and-lazy-matchheavy_minus_sign)
    - [Boundaries:no_entry:](#boundariesno_entry)
    - [Back-references](#back-references)
    - [Look-ahead and Look-behind:left_right_arrow:](#look-ahead-and-look-behindleft_right_arrow)
  - [Author](#author)

## Regex Components:jigsaw:
Regular Expressions are also considered literals, wrapping in special characters like slashes `/`. The next few sections will break <br>
down the different components of this expression.
### Anchors:anchor:
Anchors are the wrapping symbols which indicate the START and FINISH of the regular expression. <br>
 In the code snippet for validating a user's email address, the regex starts with the `^` and ends with the `$` symbol. <br> 
### Quantifiers:plus_sign:
The different quantifiers in this snippet include brackets and their contents, `{}` as well as the plus sign, `+`, and/or question mark  `?`. <br>
Brackets tell how many occurances of a character, group, <br>
 or character class must be in the input for a match to be found. <br>
 The `+` in this regex section `[a-z0-9_\.-]+` attaches it to the next part of the sequence, `)@([\da-z\.-]`.
### OR Operator:``:
An example of an OR operator would be the separator, `|` symbol. <br>
 These operators simply say that if it's present the charcters on either side of the operator would pass as a match. <br>
  For example five | 5 accepcts strings with `5` or `five`. <br>
  This regex does not show any OR operators.
### Character Classes:
Regex character classes, also known as bracket list or sets, are shown between square brackets <br> and indicate that the characters inside return in the match. <br>
 (For example if you want to match an email with  either `r` or `a` it would read something like `[ra]`.) In the email regex, the 3 sets of square brackets say the email will be verified with lowercase letters from `a` through `z`, the numbers `0,1,2,3,4,5,6,7,8,9` in the first set of brackets, and the symbols `\` and `.`, <br>
 as well as `-` and `_`. The `\d` indicates the use of digits in that section.
### Flags:triangular_flag_on_post:
 Flags, or modifiers, are _optional_ parameters that allow variation in searching. <br>
  Each flag is denoted by a single alphabetic character, like `m` or `d` modifying the expression's search behavior. <br>
  For instance `m` enables the multiline mode. `m` affects the behavior of `^` and `$` <br>
  Another example is the `g` flag. It searches for all matches in a string of e-mails.<br>
  If `g` was in the regex, which is for a global search, it will match all occurences. <br>


### Grouping and Capturing:paperclips:
Each part of the expression is sectioned off by (), brackets, braces, or symbols. <br>
It separates the address into `(letters+numbers)` `@` `(letters+numbers)` `(.2-6 letters)` <br>
 like `jsmith65@email.com`, or `l_a922@email.edu`. <br>
 A mismatch would be an email like `MayMarines-1234567@gmail.net` becuase of uppercase letters, and too may characters in the groups.

### Bracket Expressions []
Brackets `[]` indicate a SET of characters to match, with any character inside to match. <br>
The first set of brackets `([a-z0-9_\.-]+)` matches lowercase alphabetical, numerical characters, and underscores, hyphens, and periods. <br>
Curly braces `{}` are used to specify an EXACT amount of things to match. <br>
The end of the regex shows `{2,6}`. This means that the email must have at least 2 and at most 6 characters. <br>
The section `[a-z\.]{2,6}` is grouped in parenthesis after `.`, and returns `.com`, `.ru`, etc.
### :heavy_plus_sign:Greedy and Lazy Match:heavy_minus_sign:
These are quantifiers in  regex that basically shorten or elongate the string returned. <br>
The default behavior of these regexes are to be greedy, or to extract as long of a possible string version. <br> 
In this email verif snippet, the greedy match would come from the symbol `+` that appears after the first and second set of `[]`.
`^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$` <br>
Lazy, on the other hand, is simply the shortest possible string for the regex. <br>
 A lazy match could be `+?` or `*?` groupings, but in this regex we have none. <br> 
So this expression always returns the greatest possible string.
### Boundaries:no_entry:
These allow to set the start and end of the expression <br> and escape these special characters with a backslash `\`. In this regex a boundry set by `-` in `a-z0-9` to match lowercase letters and numbers, but not uppercase.
### Back-references
Back refs are more used for matching the same text previously matched by a capturing group. It helps in reusing previous parts of a pattern and in ensuring two pieces of a string match, but more useful in text or larger expressions.
### Look-ahead and Look-behind:left_right_arrow:
Lookbehind means to check what is _before_ the regex match while lookahead means checking what is _after_ your match. The presence/absence of an element before/after match item plays a role in declaring a match. <br>
**There are positive lookaheads and lookbehinds, as well as negative lookaheads and lookbehinds, but not all regex engines support them.**

## Author

 My name is Veronica Kolesnikov, a web developer from San Antonio, TX.<br>
 Currently finishing a full-stack dev bootcamp and becoming employed in front-end and/or back-end.<br>

[:octocat: Github Profile](https://github.com/verokoles)
