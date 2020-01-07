# HTML Text, CSS Introduction, and Basic JavaScript Instructions
## Text

Much of the content on a webpage is built from or involving text. Within HTML there are a few ways to designate types or levels of text. The base level is warpped in `<p>` (paragraph) tags and is used for generic copy text. To create headers or titles, you 5 different levels of `<h1>`, `<h2>`, etc. to choose from. Basic markup can be applied, using inline tags like `<b>` (bold) or `<i>` (italic).

Many of these can and should be done via CSS styling instead, but a few, such as `<abbr>` (abbreviation with on-hover tooltip), allow for uncommon but useful functionality.

## Introducing CSS

CSS provides the visual styling for web content. It is based around a simple syntax where an HTML tag, class, or id is referenced as the **selector**, and then any number of **declarations** are made, where different visual properties of the selector are assigned **values**. The simple CSS snippet below gives all HTML elements with a `<p>` tag the text color blue:

```css
p {
    color: #00f;
}
```

## Basic JavaScript Instructions

JavaScript works as a series of instructions, feeding information to the program, instructing it how to manipulate it, and returning new information back. Key pieces of information are stored in easily manipulable, named objects called **variables**. Variables must be declared and assigned a value to be useful, though that value can and probably will change as the script runs. Variables can store information typed as numbers, **strings** (text), or **booleans** (true/false values). Below are two simple variables being declared, and assigned a numerical value and a string value respectively, in two equally valid manners:

```javascript
var numberVariable = 4.3;
var stringVariable;
stringVariable = 'I am a string!';
```

**Arrays** are a form of variable that store multiple values. Individual values in an array can be accessed and edited by specifying their **index**. Below a simple matrix is created and one of its values is edited:

```javascript
var arrayVariable = ['valueA', 'valueB', 'valueC'];
arrayVariable[0] = 'valueZ';
```

The array's value after this script is run would be `['valueZ', 'valueB', 'valueC']`. Note that the index numbering of the array starts at 0, not 1.

## Decisions and Loops

Programs make basic "decisions" based on conditional statements provided to them in their code. These variants on basic "if-then/else" logic provide precise and clear instructions to the program to allow it to perform higher functions and be actually useful to anyone anywhere. In web development this logic is handled by the JavaScript.

Conditional statements read very semantically clearly, as seen in the basic example below, made to evaluate a students answer to a quiz question:

```javascript
if (studentAnswer === correctAnswer) {
    reply = 'Correct!';
} else {
    reply = 'Incorrect';
}
```

Conditionals can be given multiple criteria. An OR statement, created using pipes (`||`) between multiple criteria, return true if *any* criteria return true. An AND statement, which uses `&&` instead of pipes, only returns true if *all* criteria return true. Below is a horrid improper and grotesque example demonstrating an AND conditional and also a nested IF statement because I did the script wrong and didn't want to make another example:

```javascript
if (currentMonth === 'February' && currentDay === 28) {
    if (currentYear % 4 === 0) {
        nextDay = 29;
    } else {
        nextDay = 1;
        nextMonth = 'March';
    }
}
```

Any AND conditional can be inverted as an OR conditional with the same end functionality. The two loops below accomplish the same thing:

```javascript
if (x === 5 && y === 3) {
    z = 'Rutabaga';
} else {
    z = 'Toboggan';
}
```

```javascript
if (x !== 5 || y !== 3) {
    z = 'Toboggan';
} else {
    z = 'Rutabaga';
}
```