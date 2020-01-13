# JS Object Literals; The DOM

## The Problem Domain

Solving a problem is done in two steps. The first is to understand the problem's essense and working to outline a theoretical solution. In other words, to figure out what your finished product should look like. The second part is to create code (or whatever you're creating) that solves this problem.

So far in this class we've been working with very straightforward problems that have a very clear and simple finished product. Therefore, the codebase we've built so far is very manageable and easy to keep track of. As our projects get more complex and layered, this becomes harder to accomplish.

This means it becomes very important to understand the problem domain beforehand, and to compartmentalize your code to fit as puzzle pieces that will solve the problem. Additionally, the problem domain itself can be compartmentalized further, enabling you to solve smaller pieces of it at a time, instead of all at once.

## Object Literals

An **object** is a sort of variable which can store multiple, labeled values, called **properties** . These properties can be of any type, and can even be functions (these functions are called **methods**). The code below shows an example object.

```js
var human {
  name: 'Dave Berman',
  height: 69,
  age: 27,
  beersDrunk: 50000,
  beersPerYear: function() {
    return this.beers / this.years;
  }
}
```

In this example, `human.name` would return as `'Dave Berman'`, and `human.beersPerYear()` would return a number around 1851 ([bad example](https://www.youtube.com/watch?v=JvtRtDh3-Z8&feature=youtu.be&t=159) probably but I was committed).


## Document Object Model

The Document Object Model, or **DOM**, is a heirarchical model created based on HTML, which outlines the structure of a site. Beyond this, it provides entry points where content can be injected into objects via JS.

Objects are commonly tied to HTML content, and their properties injected onto the page using `document.getElementById()` (itself a type of method). Different methods and modifiers can be used to access different elements/sets of elements, almost like using selectors in CSS, and to store and inject data into them via JS.

The Document Object Model

This allows our site's content to be created less manually, instead using reusable techniques that will scale the site much more effectively.