# The HTML <canvas> Element and Chart.js

## The HTML <canvas> Element

The `<canvas>` element is an unusual piece of HTML which allows you to insert a space into your page's content in which you can draw content via JS. Like other tags that contain externally sourced content, like `img` or `video`, `<canvas>` is usually accompanied by a couple of attributes.

- `id` is almost always defined on a `<canvas>` element, allowing it to be easier to identify in your JS
- `width` and `height` are often set on the element as well, although they can alternatively be given by JS. These are set here because the CSS `width` and `height` properties will distort the content of a `<canvas>` drawing.

The first steps in drawing in a canvas via JS are to identify your canvas, and set the type of content it should expect:

```js
var canvas = document.getElementById('canvasId');
var ctx = canvas.getContext('2d');
```

You can draw very complex content by using properties and functions on your defined context, but outside of specialized products, content is usually inserted in a canvas via an external plugins/libraries like Chart.js. These external libraries allow you to use shorthand to define and draw a pre-defined type of content.

## Chart.js

Chart.js is a JavaScript plugin that allows you to draw charts into HTML using simple and (relatively) easy to understand code. Charts are simply objects, with data input, as well as many visual and functional customizations, defined within various properties.