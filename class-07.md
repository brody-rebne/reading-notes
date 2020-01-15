# Constructors and Prototype Functions

## JS Constructor Functions

Constructor functions serve as both a template and a method of creating JS objects. They work almost just like any other function, taking parameters and returning something to be used elsewhere—the difference being that they obviously return an object rather than a value or array. They are also called with similar syntax to a regular function (a function call: `functionName(param1, param2);` | a constructor call: `new ConstructorName(param1, param2);`—note the capitalized naming).

The parameters they take are usually assigned to property values of the object to be created, using syntax similar to how objects' properties are normally written.

A JS object:

```js
var humanN = {
  name: 'James',
  height: 12,
  children: ['Lela', 'Jacqueline'],
  species: 'human',
  function printWords(words) {
    console.log(`you asked me to print ${words}`);
  }
}
```

A constructor which could be used to generate that object:

```js
function Human(name, height, childrenArray) {
  this.name = name;
  this.height = height;
  this.children = childrenArray;
  this.species = 'human';
  this.printWords = function printWords(words) {
    console.log(`you asked me to print ${words}`);
  }
}
```

The use of `this.property` is to specify that you are setting values for properties of the object created. Equals signs and semicolons are used instead of colons and commas. The constructor name is always capitalized to easily identify what type of function it is.

## Prototype Functions

Prototype functions allow for methods to exist outside of specific constructed objects, making your objects much less memory-intensive overall and thus more scalable.

The constructor above but with the `printWords()` put into a prototype function:

```js
function Human(name, height, childrenArray) {
  this.name = name;
  this.height = height;
  this.children = childrenArray;
  this.species = 'human';
}

Human.prototype.printWords(words) {
  console.log(`you asked me to print ${words}`);
}
```

This prototype applies to any object created with `Human()` and can be called with `human.printWords('blahblahblah');` just like it could in the first example's object.