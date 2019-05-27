# Create a Style Sheet

## CSS -&gt; Style & Formatting

### Cascading Style Sheets\(CSS\) define the look and feel

Font size, font color, font type, styling around images, page layout, mouse-over effects and more are all determined by CSS.

## HTML -&gt; Structured Content

### HyperText Markup Language\(HTML\) creates the structure

HTML allows you to put images, text, videos, forms and other pieces of content together into a cohesive webpage.

## Viewing Source

To view the html of a web page, right-click and select View Source. Look for the style sheet link in the head section of your page. You can browse to the style sheet and view that as well. You can even link that style sheet to your page.

Style sheet code goes in one of three places: the page, the tag or in a file.

## Adding Style to Our Page

The following style declarations get added to our page between the `<head>...</head>` tags. It tells the browser to change the body background color to light-blue \(given by the color code \#A4F8FF\). You can look up color codes by searching for html color picker online. It also tells the browser to make the `<h1>` tag display orange text. It also tells the browser to display paragraph text as "Comic Sans MS" because we don't want to wish to be too serious. If you search for "web safe fonts" you'll find lists of fonts that most browsers can easily display.

```markup
<style>
body {
    background-color: #A4F8FF;
}

h1 {
    color: orange;
}

p {
    font-family: "Comic Sans MS";
}
</style>
```

## Your Assignment

Add the above style sheet to your page. Then change the color of the h2 tag to orange and change the color of the paragraph text to dark blue.

