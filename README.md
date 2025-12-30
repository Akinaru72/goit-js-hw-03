# Homework №3

## Instructions

- Create a repository **goit-js-hw-03** and clone it to your computer.
- In the `goit-js-hw-03` folder, create the project structure as shown in the task.

⚠️ **Pay attention!**  
File and folder names, as well as the nesting structure, must **exactly match** the specified scheme. Otherwise, the work will not be accepted.

![Project preview](assets/homework-js-3.jpg)

- Read each task carefully and complete it in the corresponding file.
- Make sure the code is formatted using **Prettier**.
- When opening the live page, there should be no errors or warnings in the console.
- Submit the homework for review.

---

## Submission Format

The homework must contain **two links**:

- a link to the source files (repository with the code);
- a link to the live page on **GitHub Pages**.

---

## Task 1. Slug Generator

**File:** `task-1.js`

Before solving the task, let’s get familiar with a new term.

**Slug** is a human-readable unique identifier used in web development to create readable URL addresses.

Have we figured this out? Now let’s finally get to the task!

### Task

Write a function `slugify(title)` that takes an article title (the `title` parameter) and returns a **slug** created from this string.

#### Requirements:

- the value of the `title` parameter is a string in which words are separated **only by spaces**;
- all characters in the slug must be in **lowercase**;
- all words in the slug must be separated by **hyphens** (`-`).

### Code for Testing

Take the code below and paste it after declaring your function to verify that it works correctly.  
The results of the function execution will be logged to the console.

```js
console.log(slugify("Arrays for beginners"));
// "arrays-for-beginners"

console.log(slugify("English for developer"));
// "english-for-developer"

console.log(slugify("Ten secrets of JavaScript"));
// "ten-secrets-of-javascript"

console.log(slugify("How to become a JUNIOR developer in TWO WEEKS"));
// "how-to-become-a-junior-developer-in-two-weeks"
```

Leave this code for the mentor to review.

### What the mentor will pay attention to during the review:

- The `slugify(title)` function is declared
- Calling `slugify("Arrays for beginners")` returns `"arrays-for-beginners"`
- Calling `slugify("English for developer")` returns `"english-for-developer"`
- Calling `slugify("Ten secrets of JavaScript")` returns `"ten-secrets-of-javascript"`
- Calling `slugify("How to become a JUNIOR developer in TWO WEEKS")` returns `"how-to-become-a-junior-developer-in-two-weeks"`

---

## Task 2. Array Composition

Complete this task in the `task-2.js` file.

Write a function called `makeArray` that takes three parameters:  
`firstArray` (an array), `secondArray` (an array), and `maxLength` (a number).

The function should create a new array that contains all elements from `firstArray`, followed by all elements from `secondArray`.

If the number of elements in the new array exceeds `maxLength`, the function should return a copy of the array limited to `maxLength` elements.  
Otherwise, the function should return the entire new array.

Take the code below and paste it after declaring your function to check that it works correctly.  
The results of the function execution will be logged to the console.

```js
console.log(makeArray(["Mango", "Poly"], ["Ajax", "Chelsea"], 3));
// ["Mango", "Poly", "Ajax"]

console.log(makeArray(["Mango", "Poly", "Houston"], ["Ajax", "Chelsea"], 4));
// ["Mango", "Poly", "Houston", "Ajax"]

console.log(makeArray(["Mango"], ["Ajax", "Chelsea", "Poly", "Houston"], 3));
// ["Mango", "Ajax", "Chelsea"]

console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 2));
// ["Earth", "Jupiter"]

console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 4));
// ["Earth", "Jupiter", "Neptune", "Uranus"]

console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus", "Venus"], 0));
// []
```

Keep this code for mentor review.

### What the mentor will pay attention to:

- The function `makeArray(firstArray, secondArray, maxLength)` is declared
- The call `makeArray(["Mango", "Poly"], ["Ajax", "Chelsea"], 3)` returns `["Mango", "Poly", "Ajax"]`
- The call `makeArray(["Mango", "Poly", "Houston"], ["Ajax", "Chelsea"], 4)` returns `["Mango", "Poly", "Houston", "Ajax"]`
- The call `makeArray(["Mango"], ["Ajax", "Chelsea", "Poly", "Houston"], 3)` returns `["Mango", "Ajax", "Chelsea"]`
- The call `makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 2)` returns `["Earth", "Jupiter"]`
- The call `makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 4)` returns `["Earth", "Jupiter", "Neptune", "Uranus"]`
- The call `makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus", "Venus"], 0)` returns `[]`
- The call to `makeArray()` with random arrays and a random number returns the correct array

---

## Task 3. Filtering an array of numbers

Complete this task in the `task-3.js` file.

Write a function `filterArray(numbers, value)` that takes an array of numbers (`numbers`) and a value (`value`) as parameters.  
The function should return a new array containing only those numbers from the `numbers` array that are greater than `value`.

### Inside the function:

- Create an empty array to store the matching numbers.
- Use a loop to iterate over each element in the `numbers` array.
- Use an `if` statement inside the loop to check each element and add it to your array if it meets the condition.
- Return the new array containing the matching numbers.

### Test code

Use the code below after declaring your function to check if it works correctly.  
The results will be logged to the console.

```js
console.log(filterArray([1, 2, 3, 4, 5], 3)); // [4, 5]
console.log(filterArray([1, 2, 3, 4, 5], 4)); // [5]
console.log(filterArray([1, 2, 3, 4, 5], 5)); // []
console.log(filterArray([12, 24, 8, 41, 76], 38));
console.log(filterArray([12, 24, 8, 41, 76], 20)); // [24, 41, 76]
```

Keep this code for mentor review.

### What the mentor will pay attention to:

- The function `filterArray(numbers, value)` is declared
- The call `filterArray([1, 2, 3, 4, 5], 3)` returns `[4, 5]`
- The call `filterArray([1, 2, 3, 4, 5], 4)` returns `[5]`
- The call `filterArray([1, 2, 3, 4, 5], 5)` returns `[]`
- The call `filterArray([12, 24, 8, 41, 76], 38)` returns `[41, 76]`
- The call `filterArray([12, 24, 8, 41, 76], 20)` returns `[24, 41, 76]`
- The call to `filterArray()` with a random array and number returns the correct array

---

**Live page: [GitHub Pages](https://akinaru72.github.io/goit-js-hw-03/)**
