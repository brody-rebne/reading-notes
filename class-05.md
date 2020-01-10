# HTML Images, CSS Color & Text

## Images

Images in HTML are created very similarly to links. To add an image in HTML, the following self-closing tag format is used:

```html
<img src='images/plantfungus.jpg' alt='Some fungus growing on the side of a plant' title='fungus on a plant' />
```

The `src` attribute, similar to the `href` attribute within `<a>` tags, provides the path to the image file to be used. In this case it points to a local file within the images folder, but it could also be pointed to an external image via a web url. The `<alt>` attribute contains text parsable by search engines. This text is also used to replace or be read alound alongside the image when the page is rendered in some accessibility or reader modes. The `<title>` tag contains the text displayed in the tooltip shown when a user hovers over the image. The `/` at the end closes the tag.

## CSS Color

Color is perhaps the most important purely cosmetic styling tool in nearly any webpage. Background, borders, and fonts can be colored to create a mood on the page, and can severely affect accessibility and usability of a site in general.

Color is used to communicate a brand image, immediately communicating visually what to feel and expect in their experience with your company or site. More practically, it can be used to direct the user's eyes to important information or action buttons, making their site journey pleasant and therefore more potentially lucrative for you.

In CSS, color is usually specified using the HEX value, a format using 3 conjoined hexadecimal based (0-F for 16 digits) numbers, for Red, Green, and Blue respectively, and ranging from 0-255, behind a # sign. Hexidecimal color values could look like `#0000ff` (pure blue), `#7d7d7d` (a medium gray) `#50fa83`, a surprisingly pleasant vibrant green. The lower the values, the darker the color.

Hex values with repeating sets of 2 digits can be expressed in only 3 digits to save time and space. For instance, the first example above could be expressed as `#00f`, or near-pure black could be written `#111'`.

## CSS Text

Along with color, styling of text is a key element of creating an intuitive visual brand. Fonts are the strongest way to communicate many elements of your brand image, letting the user know exactly who they're dealing with. A news site looking to seem more traditional, and therefore more respectable, would likely use a serifed font with an ink-printed style. A publication looking to position itself as more modern and casual might opt for a sans serif font with thicker (and more colorful) titles. For the best of both worlds, a different publication might use a slab font.

Again on the more practical side he size and flow of text can direct a user's attention to exactly what you think they ought to read and in what order.

There are many CSS styling selectors for text, styling things like the font's size, weight, border, shadow, and of course the font itself.