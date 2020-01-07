# Introductory HTML and JavaScript

## Structure

Content in documents of any kind is always presented in a purpose-built structure. For web content built from code, this structure is created using **HTML**. HTML is a markup language that uses a hierarchical tree of **tags** to describe and define objects (called **elements**), their relationships, and their place within the document. Here's an example of a simple tag: `<p>Here is some text in a paragraph</p>`. There is an opening tag `<p>`, a closing tag </p>, and the content written in between.

**Attributes** can be placed within the opening tag to set perameters for the element. Here's an example of an attribute within a simple tag, that assigns the element an ID: `<p id="elementname">Here is some text in a paragraph</p>`

A specific `id` value, or a more generic `class` value, is commonly used to reference the element (or set of elements) from the stylesheet or JavaScript.

## HTML5 Layout

The most recent version of the HTML language added a number of semantic tags that, while carrying no inherent function, help the legibility of the code by more clearly defining the type of content the element contains. This means instead of an element being nested within an unending tree of identical `<div>` tags, it can now sit within an easy-to-parse structure like this:

```html
<html>
  <body>
    <section>
      <article>
        <header>
          <nav>
            <ul>
              <li><a></a></li>
              <li><a></a></li>
            </ul>
          </nav>
        </header>
      </article>
    </section>
  </body>
</html>
```

## Process and Design

When creating a real product that fulfills a real and necessary purpose, the structure of the HTML is one of the last decisions made in designing the content. Before that, a long chain of well-researched decisions must be made to ensure that what is being built will be useful and easy to use.

The first thing to consider is what the purpose of the product is, and who would need such a product. From there, basic functionality can be determined. Once a viable set of features are outlined, the top-level structure of the product can be created. Knowing both what people will want to accomplish on your site, and how your site will accomplish it enables you to present them with the simplest and most effective journey through any necessary features. You know what content should be shown to the user at any time, and how to best show it.

Having a clear and detailed design for a product also makes it easier for it to be built, since it makes the work less open-ended and makes the functionality goals less vague.
