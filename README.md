# Coding Challenges/Algorithms/Practice Problems/What-have-you

Hi my name is Kevinn Arbas (if you haven't already noticed..Hi via my github!) and I am getting into coding through a bootcamp.  Here I just wanted to have one space where I can show the coding challenges that I've worked through from various sites, and to have a reference point later on in my career.

**Answers ahead** - please don't use this as an answer sheet for your coding challenges do the reps and get good please

---

## **'Basic' Algroithm Scripting**

---

### Convert Celcius to Fahrenheit
The formula for converting Celcius to Fahrenheit is `Celsius times 9/5, plus 32` so I did exactly that in the function 

```js
function convertToF(celsius) {
  let fahrenheit;
  fahrenheit = (celsius*(9 / 5)) + 32
  return fahrenheit;
}
```
Here were using a function declaration calling it convertToF and passing it a celsius parameter. Then initializing fahrenheit and after that assigning it to the formula mentioned above. Actually that should probably have been one line but I'll leave it for now. Then return the variable and thats it.

---

### Reverse a String 
Constraints 
- result must be a string.

```js
function reverseString(str) {
  let newArr = str.split('')
  str = newArr.reverse().join('')
  return str;
}
```
Here we pass a string to the function reverseString to reverse the string passed in.  To do that I first initialized newArr because i wanted to turn the string to an array and to that I called the .split('') method to the string to *split* up the string by each space and return an array (e.g, 'Hey' turns into ['H', 'e', 'y']). Once I had that then I reassigned the str variable to the new array with a reverse array method that reverses the array and chained on another array method that joins everything in the array with a specified empty string so there wouldn't be anything between the array elements.

---

### Return the factoral of provided interger 
Constraints
- Only intergers greater than or equal to zero will be supplied to function
- factoralize(0) = 1 

```js
function factorialize(num) {
  let prevNum = 1
  if (num > 0) {
    for (let i = 1; i <= num; i++) {
      prevNum *= i
    }
    num = prevNum
  } else if (num === 0) {
    num = 1
  }
  return num;
}
```



---

### Find the longest word in a string

constraints 
- Response should be a number

```js
function findLongestWordLength(str) {
  let newArr = str.split(' ')
  str = newArr.sort((a, b) => a.length - b.length).pop()
  return str.length;
}
```

---

## Hackerrank 30 Days of Code!

Day 1 - To complete this challenge, you must save a line of input from stdin to a variable, print Hello, World. on a single line, and finally print the value of your variable on a second line.

```js
function processData(inputString) {
    // This line of code prints the first line of output
    console.log("Hello, World.");
  
    // Write the second line of output that prints the contents of 'inputString' here.
    console.log('Welcome to 30 Days of Code!')
}
```


*A lot more to come...*