# The Regal Regex

## Summary
In short, regex is a tool for finding patterns within a string. It is most commonly used to validate user input and to search through large bodies of text. 

## Table of Contents 
- [Character Classes](#character-classes)
- [Quantifiers](#quantifiers)
- [Anchors](#anchors)
- [Lookarounds](#lookarounds)
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
Anchors help us match how items begin or end. For example: 
- ^ - Matches the beginning of the group example ^A will select every A that is at the beginning of every group.
- $ - Matches the end of a group. for example t$. In the sentance "the green hat" it would match with the t at the end of hat. 

### Lookarounds 
Look arounds are also known as look ahead or look behinds. It allows us to search for a specific word or function and match with the characters immediately before or immediately after. 
- cat(?=puppy) - would match if cat is immediately followed by puppy. 
- (?<=cat)puppy - would match if puppy is immediately preceded by puppy. 

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
