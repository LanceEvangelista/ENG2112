# ENG2112

## Alphabet Soup: Create a function that will arrange the letters of a given word to be in alphabetical order.



In order to create a function that will arrange the letters of a user
defined word into its alphabetical order the following code syntaxes are
used.


First the program asks for the word to be arranged into alphabetical order
using the 'input()' syntax. The input is stored into 'word' before being
processed and sorted.


- `word.lower()` 

The word is first shifted into lowercase to allow proper comparisson of
ASCII values as the value of ASCII letters begin with the capitalized
alphabet which give them a lower value than their lowercase counter parts.


- `list(word)`


Turns the given word example "hacker" into a list separating each letter of
the word to its own element within the list. 
Output: ['h', 'a', 'c', 'k', 'e', 'r']


- `arrange.sort()`


Sorts the elements of the specified list into alphabetical order based on the letter's given ASCII Value. For the earlier example ['h', 'a', 'c', 'k', 'e', 'r'] is sorted into ['a', 'c', 'e', 'h', 'k', 'r']


- `''.join()` 

Joins the elements of the list into a single string. ('') indicates that it will do so with no spaces in between each element.


## Emoticon Problem: Create a function that changes a specific word into an emoticon within the given phrase.

In order to create a function that replace a word within a phrase or
sentence into its corresponding emoticon the function emotify(Sentence) is used.



- `Sentence.lower()`

Shifts all the case of the words into lowercase to make sure the word corresponds with the reference word later on.

- `replace()` Replaces the word with its respective emoticon equivalent.

After being shifted to lower case the function checks if the word is present within the phrase using the following if statements.

```python
    if "smile" in Sentence:
        Sentence = Sentence.replace("smile", ":)")
    if "grin" in Sentence:
        Sentence = Sentence.replace("grin", ":D")
    if "sad" in Sentence:
        Sentence = Sentence.replace("sad", ":((")
    if "mad" in Sentence:
        Sentence = Sentence.replace("mad", ">:(")
```

using if statements instead of `elif` statements allow the program to handle scenarios wherein two different words are present within the phrase

## Unpacking List Problem: Unpack a given list into its first, middle, and last segments then print all three variables.

```python
list1 = writeyourcodehere.split()
```
- `split()` 

splits the string into a list if there are spaces or newlines in between it
considers that text as one element.

```python
i = len(list1)
```
- `len()`
Takes the length of the list which will allow the program to decide which
parts to slice later on in the program

```python
first = (list1[0])
middle =( list1[1:i-1])
last = (list1[i-1])
```

In this portion of the program each variable (first, middle, and last) is
set to the specific protions of the list they will peint later on.

Using the value `i` from `i = len(list)` the program is able to tell which
is the first element, the range of the middle elements and the last element.

Using the concept of array indexing we can easily predict which values will 
these specific portions simply by knowing how many elements are in the list.

