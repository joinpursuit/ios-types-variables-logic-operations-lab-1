# Types Variables Logic and Operations Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link of your Fork on Canvas and submit

## 1. Variable Declarations


Which of the following variables/constants are declared correctly?  Select all that apply.

```swift
a. let nameOfPrincipal: Character = "Mrs. Watkins"

b. var temperatureOutside: Int = 90.7

c. var isSummer: String = false

d. let whiteHouseAddress: Int + String = 1600 + "Pennsylvania Ave"

e. var peopleAtParty: Double = "95"
```
Answer
```swift
None of the options are declared correctly.
a. This would be a string, as it has multiple characters
b. Int does not contain decimals
c. This would a Bool
d. You cannot add differing value types (without casting/converting)
e. Doubles need to contain decimals
```

***
## 2. Boolean Evaluations 1

Which of the following expressions evaluate to true?

```swift
a. !(4 + 3 < 2 * 4)

b. !(1 + 1 != 2) && !(3 >= 3)

c. (3 < 2 || (0 < 1 && 3 >= 3)) && true

d. !!(!!true && !!false)

e. true && (true && (true && (true || false)))
```
Answer
```swift
C + E are true
```
***

## 3. Sum

You are given two variables a and b, compute their sum, store it in a variable named sum, then print the result.

```swift

Example 1
Input:
var a = 1
var b = 2

Expected values:
sum = 3

Output: 
3

Example 2
Input:
var a = 13
var b = 22

Expected values: 
sum = 35

Output:
35
```
Answer
```swift
var a = 1

var b = 2

var sum = (a + b)

print(sum)
```

***
## 4. Seconds in Year

Determine the number of seconds in a year and store the number in a variable named secondsInAYear.

```swift
Hint:
The number of seconds in a year is 365 times the number of seconds in a day.
The number of seconds in a day is 24 times the number of seconds in a hour.
The number of seconds in a hour is 60 times the number of seconds in a minute, which is 60.
```
Answer
```swift
let secHours = 60 * 60

let secDays = secHours * 24

let secYears = secDays * 365

print(secYears)
```

***
## 5. Number of Pixels

Your are given the width and height of a screen in pixels. Calculate the total number of pixels on the screen and store the result in a variable named numberOfPixels.

```swift
var width = 1920 
var height = 1080

Example 1
Input: 
var width = 4
var height = 3

Expected values:
numberOfPixels = 12

Example 2
Input:
var width = 1920
var height = 1080

Expected values:
numberOfPixels = 2073600

Hint:
Consider a 5x3 screen like this:
*****
*****
*****

The number of pixels on this screen is 5+5+5 = 5*3
```
Answer
```swift
var width = 4

var height = 3

let numberOfPixels = (width * height)

print(numberOfPixels)

var widthHD = 1920

var heightHD = 1080

let numberofHDPixels = (widthHD * heightHD)

print(numberofHDPixels)
```

***
## 6. Sum and Difference

You are given the sum and the difference of two numbers. Find out the values of the original numbers and store them in variables a and b.

```swift
let sum = 16 // a + b 
let diff = 4 // a - b

Example 1
Input: 
var sum = 16 
var dif = 4

Expected values:
a = 10
b = 6

Example 2
Input:
var sum = 2 
var dif = 0

Expected values:
a = 1
b = 1

Hint:
sum + diff = a + a + b - b
sum + diff = 2 * a
```
Answer
```swift

let sum = 16 // a + b

let dif = 4 // a - b

var a = (sum + dif) / 2

var b = sum1 - a

//This took me longer than I would like, but I think I got it.
```


***
## 7. Swap Values

Given two variable a and b, swap their values. That is the new value of a will become the old value of b and vice versa.

```swift
var a = 1
var b = 2

Example 1
Input: 
a = 2
b = 1

Hint:
Just assigning a to the value of b and b to the value of a will not work.

var a = 1
var b = 2

a = b // a will have the value 2. The original value of a is lost
b = a // b will remain the same
```
Answer
```swift
var a = 1

var b = 2

var c = g

a = b

b = c

print(a)
print(b)
```

***
## 8. Find last number

You are given a number a. Print the last digit of a.

```swift
var a = 123

Example 1
Input: 
var a = 123

Output:
3

Example 2
Input: 
var a = 337

Output:
7

Hint:
Use the remainder % operator.
```
Answer
```swift 

var j = 123

var lastDigit = (j % 10)

print(lastDigit)
```
***
## 9. Dog Years

You are given Rocky’s age in dog years. Print Rocky’s age in human years. You know that 1 human year is 7 dog years.

```swift

Example 1
Input: 
var rockysAgeInDogYears = 50

Output:
7

```
Answer
```swift
var rockysAgeInDogYears = 50

var dogYears = 7

var actualDogYears = rockysAgeInDogYears/dogYears

print(actualDogYears)
```

***
## 10. Alice's Age

x years from now Alice will be y times older than her brother Bob. Bob is 12 years old. How old is Alice?

```swift
var x = 3
var y = 2
var bob = 12

var alice = ?

Example 1
Input: 
var x = 3
var y = 2
var bob = 12

Expected values: 
alice = 27

Example 2
Input: 
var x = 1
var y = 3
var bob = 12

Expected values: 
alice = 38

Hint:
alice + x = y * (bob + x)
Solve for alice

```
Answer
```swift
var x = 3
var y = 2
var bob = 12

var alice = ((bob * y) + x)

print(alice)

// Personal note: ((bob * 2) + x) - When bob is twice as old, plus three years, this gives us alices age
```


***
## 11. Trading Oranges for Apples

You have x apples. Bob trades 3 oranges for 5 apples. He does not accept trades with cut fruit. How many oranges can you get from Bob and how many apples will you have left? The number of apples you will have left should be stored in a variable named apples. The number of oranges you will have after the trade should be stored in a variable named oranges.

```swift
var x = 17

Example 1
Input: 
var x = 17

Expected values: 
apples = 2
oranges = 9

Example 2
Input: 
var x = 25

Expected values: 
apples = 0
oranges = 15

Hint:
Use the division(/) and the remainder(%) operator

```
Answer 
```swift

var a = 17

var apples = a % 5

var oranges = (a - apples) / 5 * 3
```

***
## 12. Boy and Girl Percentages

A class consists of `numberOfBoys` boys and `numberOfGirls` girls.

Print the percentage of boys in the class followed by the percentage of girls in the class. The percentage should be printed rounded down to the nearest integer. For example 33.333333333333 will be printed as 33.

```swift
var numberOfBoys = 20
var numberOfGirls = 60

Example 1
Input: 
var numberOfBoys = 20  
var numberOfGirls = 60

Output:
25 // percentage of boys
75 // percentage of girls

```
Answer
```swift

var numberOfBoys = 20.0
var numberOfGirls = 60.0

var totalClassSize = (numberOfBoys + numberOfGirls)

var percentageOfBoys = (numberOfBoys / totalClassSize)  * 100

var percentageOfGirls = (numberOfGirls / totalClassSize) * 100

Int(percentageOfBoys)

Int(percentageOfGirls)

// - Not sure how to print as Intergers. I want to figure that out

```

***
## 13. Boolean Evaluations 2

Which of the following expressions evaluate to true?

```swift
a. false || true
b. false && true
c. !false
d. !!!true
e. !(true && true)

```
Answer
```swift
a. c. 
```

***
## 14. Boolean Evaluations 3

Which of the following expressions evaluate to true?

```swift
a. 3 < 12.3
b. 9 == 2
c. "Hello!" == "Hello!"
d. 19.0 >= 19.0
e. 9 > 7 && 7 < 10

```
Answer
```swift
a. c. d. e.
```

