# Strings Lab

Fork and clone this repo. On your fork, answer and commit the follow questions. When you are finished, submit the link to your repo on Canvas.

## Question 1

Write code that prints out all the numbers from 1 to 10 as a single string.
(Hint: the `String()` function can convert an Int to a String)

## Question 2

Write code that prints out all the even numbers from 5 to 51 as a single string.

## Question 3

Write code that prints out every number ending in 4 between 1 and 60 as a single string.

## Question 4

Print each character in the string ``"Hello world!``"

## Question 5

Print out the last character in the string below.  You cannot use the Character literal "!" (i.e you must access `myStringSeven`'s characters).

`let myStringSeven = "Hello world!"`

## Question 6

Write code that switches on a string. If the string's length is even, print out every character. If the string's length is odd, print out every other character.

## Question 7

Initialize a String with a character. Show that it is a Character, and not another String, that you're using to initialize it.

## Question 8

Build five pairs of **canonically equivalent** strings, the first of each being a pre-composed character and the second being one that uses combinable unicode scalars. Show that they are equivalent.

## Question 9

**Using only Unicode**, print out `"HELLO WORLD!"`

## Question 10

**Using only Unicode**, print out your name.

## Question 11

Print the below flower box using the following information.

- The unicode number for ⚘ is U-2698
- The top and bottom of the box are represented by dashes and the rows are |
- Use the terminator argument in your print statements to print on the same line.
- Hint: It may be useful to try printing out a box of just one character to start then work your way from there.

Flower Box:
- - - - - - - - - - -
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
- - - - - - - - - - -

## Question 12

Write a program that sets up a chess board using Unicode.

Chess Board:
♖ ♘ ♗ ♕ ♔ ♗ ♘ ♖
♙ ♙ ♙ ♙ ♙ ♙ ♙ ♙




♟ ♟ ♟ ♟ ♟ ♟ ♟ ♟
♜ ♞ ♝ ♛ ♚ ♝ ♞ ♜

## Question 13

You are given a string stored in the variable aString. Create new string named replacedString that contains the characters of the original string with all the occurrences of the character "e" replaced by "\*".

```swift
var aString = "Replace the letter e with \*"
// Your code here
 ```

Example
Input:
`var aString = "Replace the letter e with *"`

Expected values:
`replacedString = "R*plac* th* l*tt*r * with *"`


## Question 14

You are given a string stored in variable aString. Create a new string called reverse that contains the original string in reverse order. Print the reversed string.

```swift
var aString = "this string has 29 characters"
var reverse = ""

// Your code here
```

Example
Input:
`var aString = "Hello"`
Expected values:
`reverse = "olleH"`
Output:
`"olleH"`

## Question 15

Print true if aString is a palindrome, and false otherwise. A palindrome is a string which reads the same backward or forward.

```swift
let aString = "anutforajaroftuna"

// Your code here
```

Example 1
Input:
`var aString = "anutforajaroftuna"`
Output:
`true`

Example 2
Input:
`var aString = "Hello"`
Output:
`false`

## Question 16

You are given a string stored in variable problem. Write code so that you print the longest word in the string.

```swift
var problem = "find the longest word in the problem description"

// Your code here
```

Example
Input:
`var problem = "find the longest word in the problem description"`
Output:
`description`
Hint
Keep track of the longest word you encounter and also keep track of its length.

## Question 17

Given a string `testString` create a new variable called `condensedString` that has any consecutive spaces in `testString` replaced with a single space.

```swift
let testString = "  How   about      thesespaces  ?  "
//condensedString = " How about thesespaces ? "
```

## Question 18

Given a string in English, create a tuple containing the number of vowels and consonants.

```swift
let vowels = "aeiou"
let consonants = "bcdfghjklmnpqrstvwxyz"
let input = "Count how many vowels I have!"
```

## Question 19

Given a string of words separated by a `" "`. Write code that prints out the length of the last word. If there is no last word print out `"No last word"`.

Example:

Sample Input: `"How are you doing this Monday?"`

Sample Output: `7`

## Question 20

Given a string with multiple words. Write code that prints how many of them are palindromes.

Example:

Sample Input: `"danaerys dad cat civic bottle"`

Sample Output: `2`

## Question 21

You are given a string representing an **attendance record** for a student. The record only contains the following three characters:

'A' : Absent.
'L' : Late.
'P' : Present.
If a student has more than one 'A' or more than 2 continuous 'L's that student should not be rewarded. Print true if student is to be rewarded and False if they shouldn't.

Example:

Sample Input: `"PPALLP"`
Sample Output: `true`

## Question 22

Given a tuple with two strings. The first string is a **ransom note**, the second string being the characters from a magazine. Determine whether or not you can construct the ransom note using the characters from the magazine.

Each letter from the magazine can only be used once. You can assume all letters are lowercased.

Examples:

Sample Input: `("a", "b")`
Sample Output: `False`

Sample Input: `("aa", "aab")`
Sample Output: `True`