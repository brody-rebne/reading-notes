# Assorted Topics

## CSS: Images

Images (html `<img>`) can be styled with CSS much like any other HTML element. They work within the standard box model, and normal `display`, `positioning`, and `float` values apply to them as normal. Additionally, images can be used as the background of another element. Some basic selectors for using background images are:

- `background-image` - the path of the image file to be used as a background
- `background-repeat` - if and how the image will tile.
- `background-attachment` - whether the image will scroll with the page
- `background-position` - sets where on the element the image anchors to

## General: SEO

Search Engine Optimization (SEO), or how easily your site can be parsed and discovered via search engines is a deep topic that consideration must be taken for on every layer of the site. Here are some things to keep in mind to maximize SEO when building the HTML structure of a site:

1. Page `<title>` and `<meta name="description" content="Site Description Here">` are key metadata scanned for core site info
2. URL paths are also scanned for important keywords
3. The entire text of the page is scanned, but heading text is treated as more key. Consider carefully how you use `<h1>` and `<h2>`.
4. Larger bodies of text are scanned for repeated keywords. Consider repeating your header/description keywords in the text.
5. Image alt text is scanned as well, and can result in your site showing on image searches as well as web searches.