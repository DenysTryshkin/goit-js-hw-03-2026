# Homework

## Topic 4. Arrays

---

## Task 1. Slug Generator

Complete this task in the file `task-1.js`

Before solving the task, let’s define a new term!
The term slug is a human-readable unique identifier used in web development to create readable URLs.
For example, instead of seeing `mysite.com/posts/1q8fh74tx`, you can create a slug from the article title. As a result, the URL becomes more user-friendly: `mysite.com/posts/arrays-for-begginers`.

A slug is always a lowercase string where words are separated by hyphens.
Got it? Now let’s finally solve the task!

Write a function `slugify(title)` that takes an article title as a parameter `title` and returns a slug created from that string.
The value of `title` will be a string where words are separated only by spaces.
All characters in the slug must be lowercase.
All words in the slug must be separated by hyphens.

Take the code below and insert it after your function declaration to verify correctness. The results will be printed in the console.

```javascript
console.log(slugify("Arrays for begginers")); // "arrays-for-begginers"
console.log(slugify("English for developer")); // "english-for-developer"
console.log(slugify("Ten secrets of JavaScript")); // "ten-secrets-of-javascript"
console.log(slugify("How to become a JUNIOR developer in TWO WEEKS")); // "how-to-become-a-junior-developer-in-two-weeks"
```

Leave this code for mentor review.

### What the mentor will check:

* The function `slugify(title)` is declared
* Calling `slugify("Arrays for begginers")` returns "arrays-for-begginers"
* Calling `slugify("English for developer")` returns "english-for-developer"
* Calling `slugify("Ten secrets of JavaScript")` returns "ten-secrets-of-javascript"
* Calling `slugify("How to become a JUNIOR developer in TWO WEEKS")` returns "how-to-become-a-junior-developer-in-two-weeks"

---

## Task 2. Array Composition

Complete this task in the file `task-2.js`

Write a function called `makeArray` that takes three parameters: `firstArray` (array), `secondArray` (array), and `maxLength` (number). The function should create a new array containing all elements from `firstArray`, followed by all elements from `secondArray`.

If the number of elements in the new array exceeds `maxLength`, the function should return a copy of the array with a length of `maxLength` elements.
Otherwise, it should return the entire new array.

Take the code below and insert it after your function declaration to verify correctness. The results will be printed in the console.

```javascript
console.log(makeArray(["Mango", "Poly"], ["Ajax", "Chelsea"], 3)); // ["Mango", "Poly", "Ajax"]
console.log(makeArray(["Mango", "Poly", "Houston"], ["Ajax", "Chelsea"], 4)); // ["Mango", "Poly", "Houston", "Ajax"]
console.log(makeArray(["Mango"], ["Ajax", "Chelsea", "Poly", "Houston"], 3)); // ["Mango", "Ajax", "Chelsea"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 2)); // ["Earth", "Jupiter"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 4)); // ["Earth", "Jupiter", "Neptune", "Uranus"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus", "Venus"], 0)); // []
```

Leave this code for mentor review.

### What the mentor will check:

* The function `makeArray(firstArray, secondArray, maxLength)` is declared
* Calling `makeArray(["Mango", "Poly"], ["Ajax", "Chelsea"], 3)` returns ["Mango", "Poly", "Ajax"]
* Calling `makeArray(["Mango", "Poly", "Houston"], ["Ajax", "Chelsea"], 4)` returns ["Mango", "Poly", "Houston", "Ajax"]
* Calling `makeArray(["Mango"], ["Ajax", "Chelsea", "Poly", "Houston"], 3)` returns ["Mango", "Ajax", "Chelsea"]
* Calling `makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 2)` returns ["Earth", "Jupiter"]
* Calling `makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 4)` returns ["Earth", "Jupiter", "Neptune", "Uranus"]
* Calling `makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus", "Venus"], 0)` returns []
* Calling `makeArray()` with random arrays and a random number returns the correct array

---

## Task 3. Filtering an Array of Numbers

Complete this task in the file `task-3.js`

Write a function `filterArray(numbers, value)` that takes an array of numbers (`numbers`) and a value (`value`) as parameters. The function should return a new array containing only the numbers from `numbers` that are greater than `value`.

Inside the function:

* Create an empty array to store matching numbers.
* Use a loop to iterate through each element of the `numbers` array.
* Use an `if` statement inside the loop to check each element and add it to your array.
* Return the new array with the matching numbers.

Take the code below and insert it after your function declaration to verify correctness. The results will be printed in the console.

```javascript
console.log(filterArray([1, 2, 3, 4, 5], 3)); // [4, 5]
console.log(filterArray([1, 2, 3, 4, 5], 4)); // [5]
console.log(filterArray([1, 2, 3, 4, 5], 5)); // []
console.log(filterArray([12, 24, 8, 41, 76], 38)); // [41, 76]
console.log(filterArray([12, 24, 8, 41, 76], 20)); // [24, 41, 76]
```

Leave this code for mentor review.

### What the mentor will check:

* The function `filterArray(numbers, value)` is declared
* Calling `filterArray([1, 2, 3, 4, 5], 3)` returns [4, 5]
* Calling `filterArray([1, 2, 3, 4, 5], 4)` returns [5]
* Calling `filterArray([1, 2, 3, 4, 5], 5)` returns []
* Calling `filterArray([12, 24, 8, 41, 76], 38)` returns [41, 76]
* Calling `filterArray([12, 24, 8, 41, 76], 20)` returns [24, 41, 76]
* Calling `filterArray()` with random data returns the correct array
