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

/* Question #1 Answer
 
a. The constant is declared as a character, but is given a value that is a string.
b. The variable is declared as an integer, but is given a value that is a double.
c. The variable is declared as a string, but is given a value that is a bool. It also lacks the quotation marks that a proper string declaration would require.
d. The constant here is being declared as two different values.
e. The variable is declared to be of type Double, but is given a value that is a String.

None of these expressions are declared properly.
*/
```

***
## 2. Which of the following expressions evaluate to true?

```swift
a. !(4 + 3 < 2 * 4)

b. !(1 + 1 != 2) && !(3 >= 3)

c. (3 < 2 || (0 < 1 && 3 >= 3)) && true

d. !!(!!true && !!false) 

e. true && (true && (true && (true || false)))

/* Question #2 Answer

a. False
b. False
c. True
d. This expression is not syntactically correct, but if it were, it would evaluate to False.
e. True

Expressions C and E evaluate to true.
*/
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

/* Question #3 Answer

Example 1: 
Given:
var a = 1
var b = 2


var sum = a + b
print(sum)

Example 2:
Given:
var a = 13
var b = 22

var sum = a + b
print(sum)

*/
```

***
## 4.Determine the number of seconds in a year and store the number in a variable named secondsInAYear.

```swift
Hint:
The number of seconds in a year is 365 times the number of seconds in a day.
The number of seconds in a day is 24 times the number of seconds in a hour.
The number of seconds in a hour is 60 times the number of seconds in a minute, which is 60.

/* Question #4 Answer

let secondsInAMinute = 60
let secondsInAnHour = secondsInAMinute * 60
let secondsInADay = secondsInAnHour * 24
let secondsInAYear = secondsInADay * 365

*/
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

/* Question #5 Answer

Example 1
Input: 
var width = 4
var height = 3

var numberOfPixels = width * height

Example 2
Input:
var width = 1920
var height = 1080

var numberOfPixels = width * height
*/
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

/* Question #6 Answer

Example 1:
let sum = 16
let diff = 4
var a: Int
var b: Int

sum = a + b
diff = a - b
a = sum - b
diff = (sum - b) - b
diff = sum - 2b
4 = 16 - 2b
4 + 2b = 16
2b = 12
b = 6 

sum = a + b
16 = a + 6
a = 10

Example 2:
let sum = 2
let diff = 0
var a: Int
var b: Int

sum = a + b
diff = a - b
a = sum - b
diff = (sum - b) - b
diff = sum - 2b
0 = 2 - 2b
2b = 2
b = 1

sum = a + b
2 = a + 1
a = 1
*/
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

/* Question #7 Answer

Example 1:

Input:
var a = 2
var b = 1

var c: Int
c = a // a = 2, b = 1, c = 2
a = b // a = 1, b = 1, c = 2
b = c // a = 1, b = 2, c = 2

*/
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

/* Question #8 Answer

Example 1:
Input:
var a = 123
var lastDigit = a % 10
print(lastDigit)

Example 2:
Input:
var a = 337
var lastDigit = a % 10
print(lastDigit)
*/

```

***
## 9. You are given Rocky’s age in dog years. Print Rocky’s age in human years. You know that 1 human year is 7 dog years.

```swift

Example 1
Input: 
var rockysAge = 50

Output:
7

/* Question #9 Answer

Example 1
Input:
var rockysAge = 50

var rockysHumanAge = rockysAge / 7
print(rockysHumanAge)
*/

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

/* Question #10 Answer

/**************************************************************************************
Solving for Alice 

alice + x = y * (bob + x)
alice = (bob * y) + (x * y) - x
****************************************************************************************/

Example 1
Input: 
var x = 3
var y = 2
var bob = 12

var alice: Int 
alice = (bob * y) + (x * y) - x
alice = (12 * 2) + (3 * 2) - 3
alice = 24 + 6 - 3
alice = 30 - 3
alice = 27


Example 2
Input: 
var x = 1
var y = 3
var bob = 12

var alice: Int
alice = (bob * y) + (x * y) - x
alice = (12 * 3) + (1 * 3) - 1
alice = 36 + 3 - 1
alice = 39 - 1
alice = 38

*/
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

/* Question #11 Answer

var x = 17
var oranges = (x / 5) * 3
var apples = x % 5

Example 1:

var x = 17
var oranges = (x / 5) * 3
oranges = 3 * 3
oranges = 9

var apples = x % 5
apples = 17 % 5
apples = 2

Example 2:

var x = 25
var oranges = (x / 5) * 3
oranges = 5 * 3
oranges = 15

var apples = x % 5
apples = 25 % 5
apples = 0
*/

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

/* Question #12 Answer

Example 1
Input: 
var numberOfBoys: Double = 20.0  
var numberOfGirls: Double = 60.0

var totalNumberOfStudents: Double = numberOfBoys + numberOfGirls 

var placeHolderVariable = numberOfBoys / totalNumberOfStudents
var percentageOfBoys: Int = Int(placeHolderVariable * 100) // 25

placeHolderVariable = numberOfGirls / totalNumberOfStudents
var percentageOfGirls: Int = Int(placeHolderVariable * 100) // 75


print("The percentage of girls in the class is \(percentageOfGirls) and percentage of boys in the class is \(percentageOfBoys).")
*/

```

***
## 13.Which of the following expressions evaluate to true?

```swift
a. false || true
b. false && true
c. !false
d. !!!true
e. !(true && true)

/* Question #13 Answer
a. True
b. False
c. True
d. Not synatactically correct, but if it were equal to !(!(!(true))), then the expression would evaluate to False.
e. False
Expressions A and C evaluate to true.
*/

```

***
## 14.Which of the following expressions evaluate to true?

```swift
a. 3 < 12.3
b. 9 == 2
c. "Hello!" == "Hello!"
d. 19.0 >= 19.0
e. 9 > 7 && 7 < 10

/* Question #14 Answer
a. Comparison between a double and an integer causes a compiler error, but if it did compile, the expression would be True.
b. False
c. True
d. True
e. True
Expressions C,D, and E evaluate to True.
*/

```

