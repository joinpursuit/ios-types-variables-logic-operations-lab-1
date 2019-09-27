# Types Variables Logic and Operations Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link of your Fork on Canvas and submit

## 1. Which of the following variables/constants are declared correctly?  Select all that apply.

```swift
a. let nameOfPrincipal: Character = "Mrs. Watkins"

b. var temperatureOutside: Int = 90.7

c. var isSummer: String = false

d. let whiteHouseAddress: Int + String = 1600 + "Pennsylvania Ave"

e. var peopleAtParty: Double = "95"
```
E
```
```
***
## 2. Which of the following expressions evaluate to true?

```swift
a. !(4 + 3 < 2 * 4)

b. !(1 + 1 != 2) && !(3 >= 3)

c. (3 < 2 || (0 < 1 && 3 >= 3)) && true

d. !!(!!true && !!false)

e. true && (true && (true && (true || false)))
```
C, E
```
```
***

## 3. You are given two variables a and b, compute their sum and store it in another variable named sum then print the result.

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
```
```
var a = 25
var b = 35
var sum =  a + b
print("The sum of \(a) and  \(b) is \(sum)")
```
***
## 4.Determine the number of seconds in a year and store the number in a variable named secondsInAYear.

```swift
Hint:
The number of seconds in a year is 365 times the number of seconds in a day.
The number of seconds in a day is 24 times the number of seconds in a hour.
The number of seconds in a hour is 60 times the number of seconds in a minute, which is 60.
```
```
```
var secondsInAnHour = 60 * 60
var secondsInADay = secondsInAnHour * 24
var secondsInAYear = secondsInADay * 365
print("There are \(secondsInAnHour) in an hour, \(secondsInADay) in a day, and \(secondsInAYear) in a year.")
```
```
***
## 5. Your are given the width and height of a screen in pixels. Calculate the total number of pixels on the screen and store the result in a variable named numberOfPixels.

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
```
```
var width = 1920
var height = 1080
var numberOfPixels = width * height
print("If your screen is \(width) pixels by \(height) pixels, then your total number of pixels will be \(numberOfPixels)")
```
```
***
## 6. You are given the sum and the difference of two numbers. Find out the values of the original numbers and store them in variables a and b.

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
```
```
```
let sum = 16
let diff = 4

var a = (sum + diff) / 2
var b = sum - a
print("we sovled what numbers add up to \(sum), and their difference is \(diff), the two nubers are \(a) and \(b)")
```
```
```
***
## 7. Given two variable a and b, swap their values. That is the new value of a will become the old value of b and vice versa.

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
```
var a = 1
var b = 4

var changeA = b
var changeB = a

a = changeA
b = changeB
```

***
## 8. You are given a number a. Print the last digit of a.

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
Remember that a = k * (a / k) + a % k
Can you think of a value for k that gives the last digit?
```
```
var a = 123
var lastDigit = a % 10
print("The last digit in \(a) is \(lastdigit)")
```

***
## 9. You are given Rocky’s age in dog years. Print Rocky’s age in human years. You know that 1 human year is 7 dog years.

```swift

Example 1
Input: 
var rockysAge = 50

Output:
7
```

```
var rockysAgeDogYears = 50
var rockysHumanAge = rockysAgeDogYears / 7
print("Rocky's age in dog years is \(rockysAgeDogYears) and his age in human years is \(rockysHumanAge)")
```
***
## 10. Everyone hates solving word problems by hand so let’s make a program to solve them for us. 
### x years from now Alice will be y times older than her brother Bob. Bob is 12 years old. How many years does Alice have?

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
```
var x = 3
var y = 2
var bob = 12
var alice = y * (bob + x) -x
```


***
## 11. You have x apples. Bob trades 3 oranges for 5 apples. He does not accept trades with cut fruit. How many oranges can you get from Bob and how many apples will you have left? The number of apples you will have left should be stored in a variable named apples. The number of oranges you will have after the trade should be stored in a variable named oranges.

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
```
var x = 17
var apples = x % 5
var oranges = (x / 5)*3
print("If you have \(x) apples, you can get \(oranges) and have \(apples) apples left)")

```
***
## 12. A class consists of numberOfBoys boys and numberOfGirls girls.
### Print the percentage of boys in the class followed by the percentage of girls in the class. The percentage should be printed rounded down to the nearest integer. For example 33.333333333333 will be printed as 33.

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
```
var numberOfBoys = 20
var numberOfGirls = 60
var sum = numberOfBoys + numberOfGirls
var percentageOfGirls: Double = round((numberOfGirls / sum) * 100)
var percentageOfBoys: Double = round((numberOfBoys / sum) * 100)

print("With a total of \(sum) children, \(numberOfBoys) boys, \(numberOfGirls) girls; the perecentage of boys is \(percentageOfBoys), the percentage of girls is \(percentageOfGirls)")
```
***
## 13.Which of the following expressions evaluate to true?

```swift
a. false || true
b. false && true
c. !false
d. !!!true
e. !(true && true)

```
```
        
A,         
```
***
## 14.Which of the following expressions evaluate to true?

```swift
a. 3 < 12.3
b. 9 == 2
c. "Hello!" == "Hello!"
d. 19.0 >= 19.0
e. 9 > 7 && 7 < 10

```

