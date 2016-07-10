<!--{ ids:[188], language:'JavaScript', type:'workshop', order: 7, name:'Access Elements', description:'Access elements in an array with bracket notation' }-->

### Objectives

After this exercise, you should be able to:

- Access elements in an array with bracket notation

### Example

We can use dot or bracket notation to access object properties. To access array elements, however, you must use bracket notation because indices are numbers. Dot notation can only be used with valid identifiers, which cannot begin with a number.

Because arrays in JavaScript use zero-based numbering, the indices for the `fruits` array range from 0 to 2 rather than 1 to 3. To get the first element in the `fruits` array, we need to access index `0`:

```js
var fruits = ["apple", "banana", "orange"];

fruits[0]; // returns "apple"
fruits[1]; // returns "banana"
fruits[2]; // returns "orange"
fruits[3]; /* returns undefined because this index attempts
              to access a fourth element that doesn't exist */
```

Getting the last element index is a common operation to retrieve the value of the last element. To get the last element index, get the length of the array and subtract one:

```js
var lastElementIndex = fruits.length - 1;
```

Then, with bracket notation, the variable `lastElementIndex` evaluates to 2:

```js
fruits[lastElementIndex]; // returns "orange"
```

### Exercise

Create a function named `firstAndLast`. This function should:

  - take one argument, an array with at least 3 elements
  - return a new array with the first and last element of the passed array

For example:

```js
var array = ['one', 3, 'cool', 4];
firstAndLast(array); // returns ['one', 4]
```