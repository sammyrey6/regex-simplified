# REGEX SIMPLIFIED
Regular expression or regex for short is a powerful tool that allows you to look for important aspects in a string of characters. It allows you to match anything from certain characters to whitespace to even characters in a pattern. Regualr expression allows for many things but most importantly it allows for our words not to be just text on a page.
## Summary
Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

/^ and $/ basically signify the start and end of what your regex is mathcing

([a-z0-9_.-]+): This part is for the username part of the email (the part before the @ symbol).

@: This just means the @ symbol in the email address. "

([\da-z.-]+): This searches the subdomain of the email.

\.: Here, we're searching for a dot. But because dot is a special character in regular expressions, we need to put a backslash before it to make sure we find an actual dot in the text.

([a-z.]{2,6}): Finally, this part is for the website's ending, like ".com" or ".edu." We're only looking for lowercase letters and dots, and the ending should have 2 to 6 of these characters.



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

### Anchors
Anchors such as /"^","$"/ are used to search for any matches at the beggining of the string and at the end, /"\b"/ is used for matching a word boundary (the position of a word character and a non word character).
### Quantifiers
Quantifiers help you describe how many times something should appear. It's like telling your friend how many cookies they can have. For instance, * means "zero or more," + means "one or more," and ? means "zero or one." The numbers in curly braces {} help you be more specific.
### Grouping Constructs
Grouping is like putting things in a box to treat them together. When you want to find specific chunks of text, you can use ( ). It's like using a special container. But sometimes, you don't need to save what you find, so you can use (?: ) which is like a container you can see through. There are also special boxes that look ahead (?= ) or avoid certain things (?! ).
### Bracket Expressions
Bracket expressions are like secret codes for finding specific characters. It's like having a key to unlock certain characters in your text. [abc] means find either 'a', 'b', or 'c', and [^abc] means find anything except 'a', 'b', or 'c'.
### Character Classes
Character classes are like shortcuts for common things you want to find. Imagine having buttons that quickly find numbers, letters, or spaces. \d finds numbers, \w finds letters and numbers, and \s finds spaces.
### The OR Operator
The OR operator is like having a choice between two things. It's like saying, "Do you want an apple or an orange?" In regex, you use | to show this choice. (cat|dog) means "find either 'cat' or 'dog'."
### Flags
Flags are like special instructions you give to the regex. They help you search in different ways. Imagine having a pair of glasses that changes how you see things. The g flag means "search everywhere," the i flag means "ignore uppercase or lowercase," and the m flag means "look at each line separately.
### Character Escapes
Character escapes are like magic codes that let you find tricky characters. They're like a secret language that helps you find special characters like dots or parentheses. For example, \\ means "find a backslash," and \. means "find a literal dot."
## Author
https://github.com/WebDevSimplified
Web dev simplified is a web developer online teacher with videos on youtube explaining various essential web developer topics.
https://github.com/sammyrey6