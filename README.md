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
Answer: None of the variables/constants are desclared correctly
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
Answer: c; e  - evaluate to true
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
Answer:  Example 1:
               var numberA = 1
               var numberB = 2
               var sum = numberA + numberB 
               print(sum)
               Example 2:  
               var aNumber = 13
               var bNumber = 22
               var sum2 = aNumber + bNumber
               print(sum2)
               



***
## 4. Seconds in Year

Determine the number of seconds in a year and store the number in a variable named secondsInAYear.

```swift
Hint:
The number of seconds in a year is 365 times the number of seconds in a day.
The number of seconds in a day is 24 times the number of seconds in a hour.
The number of seconds in a hour is 60 times the number of seconds in a minute, which is 60.
```
Answer: 
var secondsInAMinute = 60
var minutesInAnHour = 60
var hoursInADay = 24
var daysInAYear = 365
var secondsInAYear = daysInAYear * hoursInADay * minutesInAnHour * secondsInAMinute
print(secondsInAYear)
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
Answer: var width = 1920
              var height = 1080
              var numberOfPixels = width * height 
              print(numberOfPixels)
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
Answer: 
Example 1:
let sumAandB = 16
let diffAandB = 4
let a = (sumAandB + diffAandB) / 2
print(a)
let b = sumAandB - a
print(b)
Example 2:
var sumOfAandB = 2
var diffOfAandB = 0
var A = (sumOfAandB + diffOfAandB) / 2
print(A)
var B = sumOfAandB - A
print(numberB)
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
Answer: 
var a = 1
var b = 2
var new = a
a = b
print(a)
b = new
print(b)


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
Answer: 
Example 1:
var a = 123 % 6
print(a)
Example 2:
var aNumber 337 % 33
print(aNumber)
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
Answer:
var humanYears = 1
var dogYears = humanYears * 7
var rockysAge = humanYears * dogYears
var rockysCurrentAge = 50 / dogYears
print(humanYears)
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
Answer:
Example 1:
var x = 3
var y = 2
var bob = 12
var Alice = y * (bob + x) - x
print(Alice)
Example 2:
var x = 1
var y = 3
var bob = 12
var Alice = y * (bob + x) - x
print(Alice)
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
Answer: 
Example 1: 
var x = 17
let applesTrade = 5
let oragesTrade = 3
var apples = 17 % 5
var oranges = (17 / 5) * 3
print(apples)
print(oranges)
Example 2:
var x = 25
let applesTrade = 5
let oragesTrade = 3
var apples = 25 % 5
var oranges = (25 / 5) * 3
print(apples)
print(oranges)

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
Answer:
var numberOfBoys = 20
var numberOfGirls = 60
var total = numberOfBoys + numberOfGirls

var percentageOfBoys: Double = round((Double(numberOfBoys) / Double(total)) * 100)
var percentageOfGirls: Double = round((Double(numberOfGirls) / Double(total)) * 100)
print(percentageOfBoys)
print(percentageOfGirls)

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
Answer: a; c evaluate to true
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
Answer: c; d; e
