# HTML Lists, CSS Boxes, and JS Control Flow

## HTML Lists

HTML's list tags are made for, well, listing things. There are three different types, each with similar functionality, but with different semantic purposes and different default styles.

The `<ul>`,(unordered list) tag is used to list items that are not meant to be in a specifically purposed order. A `<ul>` accepts `<li>` (list item) elements as its items, and styles them indented with bullet points. Bullet tiers can be created by nesting `<ul>`s within one another.

The `<ol>` (ordered list) tag is very similar to the `<ul>`. The difference is that, as you might expect, the items in an `<ol>` are intended to be ordered, and are styled with indented numbers. Like an `<ul>`, an `<ol>` uses `<li>`s for list items, and can be tiered in the same manner.

The `<dl>` (definition list) is slightly different. Its purpose is to define terms, as in a bibliography. Sets of `<dt>`s (definition terms) and their respective `<dd>`s (definitions) serve as list items.

## Boxes

When applying CSS to HTML, each element is treated as existing inside of a box. This box and its specific features are largely what CSS manipulates.

Each box has 4 concentric rectangles that allow CSS to manipulate its size and shape. From innermost to outermost these are:

- The object itself, defined in size by `width` and `height` (more on these later)
- `padding` - the distance between the object and its border
- `border` - the border around the object. The border's style can be manipulated in many ways using different CSS properties
- `margin` - the distance between the as-of-yet outermost edge of the box and that of any other object

As I mentioned, the basic dimensions of the box can be changed with `width` and `height`. But they can also be limited to a min or max size using `min-width`, `max-height`, etc.

Some other basic selectors used to manipulate objects are:

- `overflow` - determines how text flows when it reaches the edge of the object. Can be set to wrap within the object, clip to within the object, overflow beyond the object, and more.
- `display` - determines how the object flows within the HTML content. Many HTML elements, such as lists, are assigned default display values and must usually be overridden.
- `box-shadow` - creates a box shadow around the object.
- `visibilty` - determines whether the object is visible at all.

## Decisions and Loops

