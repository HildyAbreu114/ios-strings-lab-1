# Strings Lab 1

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit

## Question 1

Write code that prints out all the numbers from 1 to 10 as a single string.
(Hint: the `String()` function can convert an Int to a String)

var num = 1...10
for i in num {
print (" \(i)",terminator: " ")
}
***
## Question 2

Write code that prints out all the even numbers from 5 to 51 as a single string.

var num = 5...51
for i in num where i % 2==0 {
print (" \(i)",terminator: " ")
}
***
## Question 3

Write code that prints out every number ending in 4 between 1 and 60 as a single string.

var num = 1...60
for i in num where i % 10==4 {
print (" \(i)",terminator: " ")
}let 
***
## Question 4

Print each character in the string `"Hello world!"`

for (l) in "hello World" {print
print (l)
}
***
## Question 5

Print out the last character in the string below.  You cannot use the Character literal "!" (i.e you must access `myStringSeven`'s characters).

`let myStringSeven = "Hello world!"`

let myStringSeven = "Hello World!"

print(myStringSeven.last!)

***
## Question 6

Write code that switches on a string, given the following conditions:
- If the string's length is even, print out every character.
- If the string's length is odd, print out every other character.


var aString = "Pursuit"
switch aString.count % 2{
case 0:
print (aString)
default:
for (indexOf, letter) in aString.enumerated(){
if indexOf % 2 != 0{
print (letter, terminator: "")
}
}
}
***
## Question 7

Initialize a String with a character. Show that it is a Character, and not another String, that you're using to initialize it.

***
## Question 8

Build five pairs of **canonically equivalent** strings, the first of each being a pre-composed character and the second being one that uses combinable unicode scalars. Show that they are equivalent.

var sepUnicode = "\u{0065}\u{02CA}"
var combUnicode = "\u{00E9}"

var sepUnicode = "\u{0061}\u{02CA}"
var combUnicode = "\u{00E1}"

var sepUnicode = "\u{0072}\u{02CA}"
var combUnicode = "\u{0155}"

var sepUnicode = "\u{006E}\u{02CA}"
var combUnicode = "\u{0144}"

var sepUnicode = "\u{0073}\u{02CA}"
var combUnicode = "\u{015B}"
***
## Question 9

**Using only Unicode**, print out `"HELLO WORLD!"`

print ( "\u{0048} \u{0065} \u{006c} \u{006c} \u{006f}  \u{0057} \u{006f} \u{0072} \u{006c} \u{0064} \u{0021}")
***
## Question 10

**Using only Unicode**, print out your name.

print ( "\u{0048} \u{0069} \u{006c} \u{0064} \u{0079}  \u{0041} \u{0062} \u{0072} \u{0065} \u{0075}")
***
## Question 11

**Using only Unicode**, print out `"HELLO WORLD!"` in another language.

print ( "\u{0048} \u{006f} \u{006c} \u{0061}  \u{004d} \u{0075} \u{006e} \u{0064} \u{006f} \u{0021}")
***
## Question 12

Print the below flower box using the following information.

- The unicode number for ⚘ is U-2698
- The top and bottom of the box are represented by dashes and the rows are |
- Use the terminator argument in your print statements to print on the same line.
- Hint: It may be useful to try printing out a box of just one character to start then work your way from there.

```swift
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

```let 
```
var flower = "\u{2698}"
var verticalSymbol = "\u{007c}"
var horizantalSymbol = "\u{005f} "
let outline = String(repeating: horizantalSymbol, count: 11)
print(outline)

for _ in 1...7 {
for _ in 1...5 {
print("\(verticalSymbol) \(flower)", terminator: " ")
}
print(verticalSymbol)
}
print(outline)```

***
## Question 13

Write a program that sets up a chess board using Unicode.
```
```swift
Chess Board:
♖ ♘ ♗ ♕ ♔ ♗ ♘ ♖
♙ ♙ ♙ ♙ ♙ ♙ ♙ ♙




♟ ♟ ♟ ♟ ♟ ♟ ♟ ♟
♜ ♞ ♝ ♛ ♚ ♝ ♞ ♜

````

let  piece1 = "\u{2656}  \u{2658}  \u{2657}  \u{2655}  \u{2654}  \u{2657}  \u{2658}  \u{2656}"

let piece2 = "\u{2659}  \u{2659}  \u{2659}  \u{2659}  \u{2659}  \u{2659}  \u{2659}  \u{2659}"


let piece3 = "\u{265F}  \u{265F}  \u{265F}  \u{265F}  \u{265F}  \u{265F}  \u{265F}  \u{265F}"

let piece4 = "\u{265C}  \u{265E}  \u{265D}  \u{265B}  \u{265A}  \u{265D}  \u{265E}  \u{265C}"


for i in 1...8 {
if i == 1{
print (piece1)
}
else if i == 2 {
print (piece2)
}
else if i == 7{
print (piece3)
}
else if i == 8{
print (piece4)
} else {
print ("")
}
}
```

***
## Question 14

You are given a string stored in the variable `aString`. Create new string named `replacedString` that contains the characters of the original string with all the occurrences of the character `"e"` replaced by `"\*"`.

```swift
var aString = "Replace the letter e with \*"
// Your code here
 ```

Example:

Input:
`var aString = "Replace the letter e with *"`

Expected values:
`replacedString = "R*plac* th* l*tt*r * with *"`

var aString = "Replace the letter e with *"
var replacedString = aString.replacingOccurrences(of: "e", with: "*")
print(replacedString)***

## Question 15

You are given a string stored in variable `aString`. Create a new string called `reverse` that contains the original string in reverse order. Print the reversed string.

```swift
var aString = "this string has 29 characters"
var reverse = ""

// Your code here
```

Example:
Input:
`var aString = "Hello"`

Output:
`"olleH"`

var aString: String = "this string has 29 characters"
print (String(aString.reversed()))
***
## Question 16

You are given a string stored in variable `aString`. Print `true` if `aString` is a palindrome, and `false` otherwise. A **palindrome** is a string which reads the same backward or forward.

```swift
let aString = "anutforajaroftuna"

// Your code here
```

Example 1:
Input:
`var aString = "anutforajaroftuna"`

Output:
`true`

Example 2:
Input:
`var aString = "Hello"`

Output:
`false`

********** NOT SURE WHY IT RUNS SO MANY TIMES************
let aString: String = "anutforajaroftuna"
var reverse = String(aString.reversed())

for word in aString {
for word1 in reverse {
if word == word1 {
print (true)
}else {
print (false)
}
}
}
***
## Question 17

You are given a string stored in variable `problem`. Write code so that you print each word of the string on a new line.

```swift
var problem = "split this string into words and print them on separate lines"

// Your code
```

Example:
Input:
`var problem ="split this string into words and print them on separate lines"`

Output:
```swift
split
this
string
into
words
and
print
them
on
separate
lines
```

var problem = "split this string into words and print them on separate lines"
var problemArr = problem.split(separator: " ")
print (problemArr)
for i in problemArr {
print (i)
}

***
## Question 18

You are given a string stored in variable `problem`. Write code that prints the longest word in the string.

```swift
var problem = "find the longest word in the problem description"

// Your code here
```

Example:
Input:
`var problem = "find the longest word in the problem description"`

Output:
`description`

Hint: Keep track of the longest word you encounter and also keep track of its length.

***
## Question 19

Given a string in English, create a tuple containing the number of vowels and consonants.

```swift
let vowels = "aeiou"
let consonants = "bcdfghjklmnpqrstvwxyz"
let input = "Count how many vowels I have!"
```

***
## Question 20

Given a string of words separated by a `" "`. Write code that prints out the length of the last word.

If there is no last word print out `"No last word"`.

Example:
Input: `"How are you doing this Monday?"`

Output: `7`

***
