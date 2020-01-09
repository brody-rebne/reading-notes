# HTML Links, CSS Layout, JS Functions

## Links

The HTML `link` attribute allows you to create **hypertext** that will send the user to other webpages (as well as other less common functionality) on click. Links in HTML are by standard created using `<a>` (anchor) tags with an attribute `href="linkhere"` (href for hypertext reference). The text content inside the tag forms the display text for the link; the link itself is set as the href's value.

Links can be used to link to external urls, or just pages within the same local site. When your site is accessed publically, different pages' urls are determined by the filepath in the sites directory. This means that directory folders with public-facing content should be named and organized with clarity and efficiency.

## Layout

Layout in CSS concerns the size and shape of different elements' boxes, as well as how they flow in the page and interact with eachother. Much of layout functionality is accomplished by creating container boxes for groups of elements, and determining how each level of nested boxes should be spaced, aligned, and sized. A key selector in creating a proper layout is `position`. The most common `position` values and their purposes include:

- `normal` - the position of the element follows the default given to it by its HTML
- `absolute` - the position of the element is to be set relative to the boundings of its containing element
- `relative` - the position of the element is to be set relative to where its default positioning would be
- `fixed` - the position of the element is to be set relative to the viewport, and will not move when its container's properties are changed, nor when the user scrolls the page

## Functions

In JavaScript, a function is simply a set of commands that return a value, that can be easily be reused elsewhere in the JS. Any types of commands can be run in the function, and any necessary input can be taken in according to a defined format as **parameters** any time the function is called. A simple hypothetical function call to get a user's answer to a specific question could look like this:

```js
findAnswer(brody, questionC);
```

In this example, `findAnswer()` is the function being called, whi;e `brody` and `questionC` are the parameters specifying which user/question coordinate should be returned.

## Pair Programming

Pair Programming is a standard format for collaborative code. Collaboration is vital to nearly any type of work, and development is certainly no exception. However, since it's not helpful to have multiple people typing on the same keyboard, people have found a better way to best enable two developers to work symbiotically.

The standard method is to have one person "driving"—typing code out and managing smaller-scale, practical solutions, while the other "navigates"—providing higher-level direction and managing strategic goals and solutions.

This system allows both people to stay focused on one domain of problems, without having to stop and go working out minor details in an enormous scope of concerns.

Pair Programming also aids learning. By communicating our creative solutions and thought processes with eachother, we both learn from eachother and reinforce our existing knowledge.