# Matching an email 

Welcome to this comprenensive tutorial on matching email regular expressions (regex) using JavaScript in the field of Computer Science. Upon completing the tutorial, both newcomers and academics alike will have a clear comprehension and understanding of regex components, achieved through detailed explanations and example analysis. In this tutorial, we will delve into email regex, breaking down the components of a regex pattern designed to validate email adresses and explaining how each part contributes to ensuring accurate and reliable email validation.

## Summary

Throughout this tutuorial, the featured regualr expression (regex) as seen below, will be refrenced for analysis in regards to each regex component to ensure new-comers and academics alike are able to undesrtand and grasp material with absolute clarity. THe regex components discussed in this document imclude: anchors, quantifiers, grouping constructs, bracket expressions, character classes, the OR operator, flags, and characters escapes.

regex:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents: Regex Components

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

### Anchors

Regular expressions are powerful tools for matching patters in text Anchors, which are special characters in regular expressions, play an essentiaal role in defining the position of the pattern within the input string. In the context of email validation, like in the regex featured in this tutuorial /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/, it is crucuial to ensure that the entire input string matches the specified patter, rather than just a part of it.

### Quantifiers

In regular expressions, quantifiers are used to specify how many times a pattern should match. Quantifiers are placed after a character, character class, or group, in order to determine the minimum and maximum number of times preceding patterns should occur.

the + quantifier means "one or more," and is usede after the pattern [a-z0-9_\.-] in the first capturing group ([a-z0-9_\.-]+). This indicates that the pattern [a-z0-9_\.-] should occur at least once, but it can also occur multiple times consecutively. Thus, the group will match one or more lowercase letters, digits, underscores, dots, or hyphens.

### OR Operator

Alternation is the term in regular expression that is actually a simple “OR”. In a regular expression it is denoted with a vertical line character | . For instance, we need to find programming languages: HTML, PHP, Java or JavaScript

### Character Classes

Character classes, known as character sets are a shot and more concise regular expressions that represent specific sets of characters. Through the use of character classes, you can simplify and shorten regex patterns, thereby making them readable and easier to understand.

in our regex in this tutorial:  /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ uses various regex elements, including character classes, character sets, metacharacters, and repeating character classes. These elements ensure the regex and assesed and sourced accurately to match the email addresses.

### Flags

A flag is an optional parameter to a regex that modifies its behavior of searching. A flag changes the default searching behavior of a regular expression. It makes a regex search in a diffirent way. A flag is a denoted using a single lowercase alphabetic character in JavaScript regex, we have a total of 6 flags, each serving a diffirent purpose.
for an expression created literslly, i.e. using the forward slashes //, flags comes after the second slash. 

### Grouping and Capturing

Groups group multiple patterns as a whole, and capturing groups provide extra submatch information when using a regular expression pattern to match against a string. Backreferences refer to a previously captured group in the same regular expression.

Capturing groups are a way to treat multiple characters as a single unit. They are created by placing the characters to be grouped inside a set of parentheses. For example, the regular expression (dog) creates a single group containing the letters "d" "o" and "g" .

### Bracket Expressions

Bracket expressions are a fundemental concept in rewgular expressions, used to define a set of characters that can be matched within a single position in a text string. They are denoted by square brackets [...], and any character enclosed within these brackets will become a part of the allowed set. Bracket expressions can contain individual characters, and even define character ranges using a hyphen, such as a-z for all lowercase letters or 0-9 for digits. Whats the purpose? the bracket expressions create flexible patterns that match various combinations of characters in your target text.

### Greedy and Lazy Match

Greedy means your expression will match as large a group as possible, lazy means it will match the smallest group possible. For this string: abcdefghijklmc. and this expression: a.*c. A greedy match will match the whole string, and a lazy match will match just the first abc 

### Boundaries

A word boundary assertion checks if the current position in the string is a word boundary. A word boundary is where the next character is a word character and the previous character is not a word character, or vice versa. 

\b asserts that the current position in the string is a word boundary. \B negates the assertion: it asserts that the current position is not a word boundary. Both are assertions, so unlike other character escapes or character class escapes, \b and \B don't consume any characters.

A word character includes the following:

Letters (A–Z, a–z), numbers (0–9), and underscore (_).
If the regex is Unicode-aware and the i flag is set, other Unicode characters that get canonicalized to one of the characters above through case folding.

### Back-references

A backreference is a way to match the same text as previously matched by a capturing group. Capturing groups count from 1, so the first capturing group's result can be referenced with \1, the second with \2, and so on. \0 is a character escape for the NUL character.

In case-insensitive matching, the backreference may match text with different casing from the original text. The backreference must refer to an existent capturing group. If the number it specifies is greater than the total number of capturing groups, a syntax error is thrown.

### Look-ahead and Look-behind

A lookahead assertion "looks ahead": it attempts to match the subsequent input with the given pattern, but it does not consume any of the input — if the match is successful, the current position in the input stays the same. A regular expression generally matches from left to right. This is why lookahead and lookbehind assertions are called as such — lookahead asserts what's on the right, and lookbehind asserts what's on the left.

In order for a (?=pattern) assertion to succeed, the pattern must match the text after the current position, but the current position is not changed. The (?!pattern) form negates the assertion — it succeeds if the pattern does not match at the current position.

## Author

Follow me on github github.com/Cbaca4

Deployed Github-gist link: https://gist.github.com/Cbaca4/c6cef95a5934823accde38fdc5d758b9

Github repository: https://github.com/Cbaca4/Regex-Tutorial-in-JS
