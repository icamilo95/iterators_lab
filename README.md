# Iterators Lab

### Description

In the iterators lab we will be continuing our exploration of
iterators. We have a series of challenges that require you to use the
iterators we discussed in class. We will try to use various testing
methods to verify that your code is working.

### Phase-1

Research the following term and summarize your findings on it two to
three sentences:

* `higher-order function`


Update this README with a description of each of the following and an
example you've created:

* `forEach`: [Runs a loop throught all the elements of the array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)

* `map`: [Runs a loop throught all the elements of the array and returns a new array with all the values (now) affected by the function called](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
		

* `filter`: [Returns (new array with) the elements of the array that meet the condition] (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)
			
* `reduce`: [Returns a new array with only one value. It accumulates the value returning from the function ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reduce)
			 
* `some`: [Returns true if at least one the elements meets the condition, otherwise returns false ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/some)

* `every`: [Returns true only if all the elements meet the condition, otherwise returns false ](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/every)

Use the notes provided to help guide you explanation.

### Phase-2

<!-- DONE -->
* Run `npm install` from the `iterators_lab` directory.
<!-- DONE -->
* Looks at the tests we've written in the `test` folder. Run the tests
  with `npm test` (also from the `iterators_lab` directory). They
  should all fail.
<!-- DONE -->
* Get all of the tests to pass by writing the necessary code in
  `src/iterators.js`.

### Phase-3

Refactor the following code using `map` to make only one call to the `map` function versus the two below.

<!-- -ANSWER- -->
var myNumbers = [ -1, 2, -3, 4, -5, 6];

var square = function(num) {
	return num * num;
};

var sqrRoot = function(num) {
	return Math.sqrt(square(num));
};


// var sqrNumbers = map(myNumbers, square);
var absNumbers = myNumbers.map(sqrRoot);





<!-- ```
var myNumbers = [ -1, 2, -3, 4, -5, 6];

var square = function(num) {
	return num * num;
};

var sqrRoot = function(num) {
	return Math.sqrt(num);
};


var sqrNumbers = map(myNumbers, square);
var absNumbers = map(sqrNumbers, sqrRoot);
```
 -->



