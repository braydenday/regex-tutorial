# Regex Tutorial on validating input for emails

Regular expressions have the capability to identify specific character patterns within a string. Additionally, they enable the discovery and substitution of individual characters or character sequences within the string. These expressions are commonly employed for input validation purposes. In this case, the regular expression is designed to identify character patterns corresponding to valid email addresses.

## Summary

This is the regex code that we will be anaylizing today is: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

The anchors used to contain this regular expression are: ^ to start, and $ to finish.

### Quantifiers

In this instance, the plus sign (+) was employed to indicate the presence of an additional sequence that requires matching, serving as a representation of a greedy quantifier. Furthermore, we utilized the range specification {2,6} as another form of greedy quantifier, dictating that the input must consist of a minimum of 2 characters and up to a maximum of 6 characters.

### Character Classes

Within this particular regular expression, the character class \d is implemented, and in the context of JavaScript, it designates the inclusion of any digit spanning from 0 to 9.

### Grouping and Capturing

This example involves the capturing of three distinct groups. The initial group, labeled as Group #1, encompasses the email account's username, represented by the pattern [a-z0-9_.-]. The subsequent group gathers the domain name or the email service being utilized, as denoted by [\da-z.-]. Lastly, the third group focuses on capturing the domain extension (such as .com or .net), stipulated by [a-z.]{2,6}.

### Bracket Expressions

Similar to the groups presented in this instance, there are also three sets of bracket expressions. These bracket expressions enclose information within square brackets, such as [], to specify permissible content for matching.

Bracket Expression #1: [a-z0-9_.-] - comprises characters that are case-sensitive, spanning from a to z, numbers from 0 to 9, underscores, periods, and hyphens.

Bracket Expression #2: [\da-z.-] - encompasses all digits, along with case-sensitive characters ranging from a to z, in addition to periods and hyphens.

Bracket Expression #3: [a-z.] - encompasses characters that are case-sensitive, covering the range from a to z, as well as periods.

### Greedy and Lazy Match

Within this illustration, we exclusively utilized greedy quantifiers + and {}. This choice enables the matching process to expand freely until the necessary condition is met. Alternatively, if these quantifiers were employed as lazy quantifiers, they would take the form of +? or {}?. These adjustments would prompt the system to identify the shortest possible match instead.

## Author

My name is Brayden Day, and I finally can understand how to code!

Here is my github repository: https://github.com/braydenday
