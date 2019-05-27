# Span and Div Tags

Span and Div are container tags that define parts of your document. They are great for applying styles to a section of text. They are also helpful for dividing your document into parts such as header, body and footer.

* The &lt;span&gt; tag is used to group inline-elements in a document.
* The &lt;span&gt; tag provides no visual change by itself.
* The &lt;span&gt; tag provides a way to control the style of part of your document.
* The &lt;div&gt; tag defines a section of an HTML document.
* The &lt;div&gt; tag is used to group elements to format them with CSS.
* You can make a &lt;span&gt; or &lt;div&gt; point to a style sheet using the `id` or `class` attribute.
* The `id` must be unique. There can only be one element with that particular id.
* The `class` attribute can apply to in different elements.

```markup
<span style="color:ff0000">This text is red</span> this text isn't red.
<div style="color:#0000ff">
  <h3>This is a heading</h3>
  <p>This is a paragraph.</p>
</div>
```

## Attributes

The &lt;span&gt; and &lt;div&gt; tags have no _required_ attributes but the most common attributes used are:

* **style** - specifies a style that applies to all content and elements up to the end tag
* **class** - specifies a CSS classs that applies to all content and elements up to the end tag
* **id** - identifies the tag so you can select it with jQuery or JavaScript

In general, use `id` whenever you want to refer to a specific element and `class` when you have a number of things that are alike.

