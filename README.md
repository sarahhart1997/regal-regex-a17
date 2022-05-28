# The Regal Regex

## Summary
In short, regex is a tool for finding patterns within a string. It is most commonly used to validate user input and to search through large bodies of text. 

## Table of Contents 
- [Character Classes](#character-classes)
- [Quantifiers](#quantifiers)
- [Anchors](#anchors)
- [Lookarounds](#lookarounds)
- [Modifiers](#modifiers)
- [Logical OR](#logical-or)
- [Flags](#flags)

## Regex Componets
Now that we understand the valuable uses of these functions let's learn how to use them! 

### Character Classes
Character classes search for patterns based on the what that item is. Instead of trying to match specific characters or patterns. Common examples of this include: 
- /d - Matches any number (0-9)
- /w - Matches any word
- [] - Allows you to match custom character sets such as [A-D]. Search for every instance of that character [ABC] seperately or adding ^ will match every character except A, B and C in [^ABC]

### Quantifiers 
Quantifiers appear after a pattern and set the limits or boundaries that must be fufilled in order for that string to be matched. 

- ? = Allows a pattern 0 or 1 times
- * = Allows 0 or many times
- + = Allows 1 or more times 
- {min, max} = explicit counts of pattern

### Anchors
### Lookarounds
### Modifiers

### Logical OR and Grouping
A vertical bar or | is used a logical OR this allows us to search for data that could appear in different orders. This is often used with () or grouping to provide the most useful matches. 

For example: 
(Dog | Puppy) Cat
Will find every example of a dog or puppy paired with a cat. 

While: 
(Dog | Cat) Puppy
Will find every instance of a dog or cat paired with a Puppy. 

### Flags
By default regex expressions search for the first match. However, you can change this behavior by adding flags such as: 
- g = global search
- i = case does not matter, will return everything of that letter.

## Author
This tutorial was written by Sarah Hart an entertainment technology professional and web designer based out of Hoboken, New Jersey. Sarah's work can be found at: https://github.com/sarahhart1997 
