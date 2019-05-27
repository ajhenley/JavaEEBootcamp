# HTML,CSS and Javascript

## Three languages all web developers must learn:

* **HTML** to define the content of web pages
* **CSS** to specify the layout of web pages
* **JavaScript** to program the behavior of web pages

HTML \(HyperText Markup Language\) is the primary markup language used in web pages. Web pages consist of content \(text and images\) and markup \(tags\). The browser renders the tags to format the content.

## Before we start

To create and test HTML pages, you need a text editor and a web browser. Notepad++ or GEdit or Kate will work for our purposes because they highlight HTML markup with colors to make it easier to read.

Use the web browser to preview your documents as you work. It's a good idea to test your documents in different browsers. Each browser has slightly different rendering and other quirks. The most common browsers are Google Chrome, Mozilla Firefox, Microsoft Internet Explorer, Safari, and Opera.

## A simple document

Let's start with a simple document. Write this code in your editor \(or copy-and-paste it\), and save it as "index.html". Save the file with the correct extension so it displays as intended.

```markup
<!DOCTYPE html>
<html>
  <head>
    <title>Simple document</title>
  </head>
  <body>
    <h1>This is my heading</h1>
    <p>This is some text in a paragraph that will be seen by viewers.</p>
  </body>
</html>
```

Now open the document in your browser and look at the result. From the above example, we can deduce certain essentials of an HTML document:

* The first line with `<!DOCTYPE html>` declares the type of the document.
* The HTML document begins with a `<html>` tag and ends with its counterpart, the `</html>` tag.
* Within the `<html></html>` tags, there are two main pairs of tags, `<head></head>` and `<body></body>`.
* Within the `<head></head>` tags, there are the `<title></title>` tags which enclose the textual title to be shown in the title bar of the web browser.
* Within the `<body></body>` is a paragraph marked by a `<p></p>` tag pair.

