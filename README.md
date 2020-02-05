# JavaScript


## Closures, Scope, and Execution Context

* Challenge 1
Create a function createFunction that creates and returns a function. When that created function is called, it should print “hello”.
```
const  function1 = createFunction();
// now we’ll call the function we just created
function1(); //should console.log(‘hello’);
```

When you think you completed createFunction, un-comment out those lines in the code and run it to see if it works.

* Challenge 2
Create a function createFunctionPrinter that accepts one input and returns a function. When that created function is called, it should print out the input that was used when the function was created.

```
const printSample = createFunctionPrinter(‘sample’);
const printHello = createFunctionPrinter(‘hello’)
// now we’ll call the functions we just created
printSample(); //should console.log(‘sample’);
printHello(); //should console.log(‘hello’);
```


* Challenge 3
Examine the code for the outer function. Notice that we are returning a function and that function is using variables that are outside of its scope.
Uncomment those lines of code. Try to deduce the output before executing.

* Challenge 4
Now we are going to create a function addByX that returns a function that will add an input by x.

```
const addByTwo = addByX(2);
addByTwo(1); //should return 3
addByTwo(2); //should return 4
addByTwo(3); //should return 5

const addByThree = addByX(3);
addByThree(1); //should return 4
addByThree(2); //should return 5

const addByFour = addByX(4);
addByFour(4); //should return 8
addByFour(10); //should return 14
```


* Extension: Challenge 5
Write a function once that accepts a callback as input and returns a function. When the returned function is called the first time, it should call the callback and return that output. If it is called any additional times, instead of calling the callback again it will simply return the output value from the first time it was called.

* Extension: Challenge 6
Write a function after that takes the number of times the callback needs to be called before being executed as the first parameter and the callback as the second parameter.

* Extension: Challenge 7
Write a function delay that accepts a callback as the first parameter and the wait in milliseconds before allowing the callback to be invoked as the second parameter. Any additional arguments after wait are provided to func when it is invoked. HINT: research setTimeout();

* Extension: Challenge 8
Write a function rollCall that accepts an array of names and returns a function. The first time the returned function is invoked, it should log the first name to the console. The second time it is invoked, it should log the second name to the console, and so on, until 


## Asynchronicity

* Challenge 1
Thinking point (no writing code necessary for this challenge): Inspect the code given to you in Challenge 1. In what order should the console logs come out? Howdy first or Partnah first?
* Challenge 2
Create a function delayedGreet that console logs welcome after 3 seconds.
* Challenge 3
Create a function helloGoodbye that console logs hello right away, and good bye after 2 seconds.
* Challenge 4
Create a function brokenRecord that console logs hi again every second. Use the End Code button to stop the console logs when you are satisfied that it is working.
* Challenge 5
Create a function limitedRepeat that console logs hi for now every second, but only for 5 seconds. Research how to use clearInterval if you are not sure how to do this.
* Challenge 6
Write a function called everyXsecsForYsecs that will accept three arguments: a function func, a number interval, and another number duration. everyXsecsForYsecs will execute the given function every interval number of milliseconds, but then automatically stop after duration milliseconds. Then pass the below sayHi function into an invocation of everyXsecsForYsecs with 1000 interval time an 5000 duration time. What do you expect to happen?
* Challenge 7
Write a function delayCounter that accepts a number (called ‘target’) as the first argument and a number of milliseconds (called ‘wait’) as the second argument, and returns a function. When the returned function is invoked, it should log to the console all of the numbers between 1 and the target number, spaced apart by ‘wait’ milliseconds.


