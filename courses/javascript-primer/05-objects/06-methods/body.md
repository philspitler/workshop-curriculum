<!--{ ids:[179], language:'JavaScript', type:'workshop', order: 5, name:'Methods', description:'Even functions can be a value' }-->

### Objectives

After this exercise, you should be able to:

- Demonstrate how to assign a function as the value of a property
- Demonstrate how to call a method

### Example

When the value of a property is a function, it's known as a __method__. To demonstrate, we'll create an object named `student` and give it a method named `learn`:

```js
var student = {
  learn: function(subject) {
    return "I'm learning " + subject + "!";
  }
};
```

`learn` is the name of the property, and the property is assigned an anonymous function. Similar to function expressions, however, the function does not need to be anonymous – you can name the function.

Calling a method is the same as calling a function, except you call a method by using dot notation and reference the parent object:

```js
student.learn("JavaScript"); // returns "I'm learning JavaScript!"
```

In general, write method names the same as you would any other function – with action word(s) that describe what the function does.

### Exercise

Add a method to the `orange` object named `peel`. This method should take no arguments and return the string `"Delicious!"`.

Once you've created the method, call the method and assign the method call to the variable `snackTime`. When complete, `snackTime` should have a value of `"Delicious!"`.
