# Coding Challenges/Algorithms/Practice Problems/What-have-you

Hi my name is Kevinn Arbas (if you haven't already noticed..Hi via my github!) and I am getting into coding through a bootcamp.  Here I just wanted to have one space where I can show the coding challenges that I've worked through from various sites, and to have a reference point later on in my career.

**Answers ahead** - please don't use this as an answer sheet for your coding challenges do the reps and get good please

---

## **'Basic' Algroithm Scripting**

---

### Convert Celcius to Fahrenheit
The formula for converting Celcius to Fahrenheit is `Celsius times 9/5, plus 32` so I did exactly that in the function 

```
function convertToF(celsius) {
  let fahrenheit;
  fahrenheit = (celsius*(9 / 5)) + 32
  return fahrenheit;
}
```
Here were using a function declaration calling it convertToF and passing it a celsius parameter. Then initializing fahrenheit and after that assigning it to the formula mentioned above. Actually that should probably have been one line but I'll leave it for now. Then return the variable and thats it.

---

### Reverse a String 
Constraints - result must be a string.

```
function reverseString(str) {
  let newArr = str.split('')
  str = newArr.reverse().join('')
  return str;
}
```
Here we pass a string to the function reverseString to reverse the string passed in.  To do that I first initialized newArr because i wanted to turn the string to an array and to that I called the .split('') method to the string to *split* up the string by each space and return an array (e.g, 'Hey' turns into ['H', 'e', 'y']). Once I had that then I reassigned the str variable to the new array with a reverse array method that reverses the array and chained on another array method that joins everything in the array with a specified empty string so there wouldn't be anything between the array elements.
