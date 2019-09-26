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

THE ANSWER IS 

NONE ARE DECLARED CORRECTLY


***
## 2. Which of the following expressions evaluate to true?

```swift
a. !(4 + 3 < 2 * 4)

b. !(1 + 1 != 2) && !(3 >= 3)

c. (3 < 2 || (0 < 1 && 3 >= 3)) && true

d. !!(!!true && !!false)

e. true && (true && (true && (true || false)))
```

THE ANSWER IS 

C and E


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
THE ANSWER IS

var a = 1

var b = 2
var sum = a + b

print(sum)


***
## 4.Determine the number of seconds in a year and store the number in a variable named secondsInAYear.

```swift
Hint:
The number of seconds in a year is 365 times the number of seconds in a day.
The number of seconds in a day is 24 times the number of seconds in a hour.
The number of seconds in a hour is 60 times the number of seconds in a minute, which is 60.
```

THE ANSWER IS
var SecondsInMinute = 60
var SecondsInHour = SecondsInMinute * 60
var SecondsInDay = SecondsInHour * 24
var secondsInAYear = SecondsInDay * 365


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

THE ANSWER IS

var width = 1
var height = 2
var numberOfPixels = width * height


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

THE ANSWER IS

var sum = 2
var dif = 0

var a = (sum + dif ) / 2
var b = a - dif

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
THE ANSWER IS

var a = 2
var b = 1
let aDontChange = a

a = b
b = aDontChange

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

THE ANSWER IS

var a = 1234
var lastN = a%10
print(lastN)


***
## 9. You are given Rocky’s age in dog years. Print Rocky’s age in human years. You know that 1 human year is 7 dog years.

```swift

Example 1
Input: 
var rockysAge = 50

Output:
7

```

THE ANSWER IS

var rockysAge = 64
var hYear = rockysAge / 7
print("rocky is \(rockysAge) in dog years, rocky is \(hYear) in human years")


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

THE ANSWER IS

var x = 1
var y = 3
var bob = 12
var alice = 0

alice = (y * (bob + x)) - x
print(alice) 

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

THE ANSWER IS

var input = 25
var BOT = input / 5
var oranges = BOT * 3
var apples = input % 5
print("you have \(apples) apples left and \(oranges) oranges after starting with \(input) apples" )


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

THE ANSWER IS 

var numberOfBoys: Double = 20
var numberOfGirls: Double = 60
var total = numberOfBoys + numberOfGirls
var dofb = numberOfBoys / total
var dofg = numberOfGirls / total
var pofb = dofb * 100
var pofg = dofg * 100


***
## 13.Which of the following expressions evaluate to true?

```swift
a. false || true
b. false && true
c. !false
d. !!!true
e. !(true && true)

```


THE ANSWER IS 
A and C 

***
## 14.Which of the following expressions evaluate to true?

```swift
a. 3 < 12.3
b. 9 == 2
c. "Hello!" == "Hello!"
d. 19.0 >= 19.0
e. 9 > 7 && 7 < 10

```
THE ANSWER IS 
C, D AND E

