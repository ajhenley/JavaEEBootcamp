# More to Say About Styles

An inline style will override the styles declared in your head tags which override those in the external file. Let's change the first paragraph to illustrate this.

```markup
<p style="color">This paragraph text would be blue even if there is a different setting on the page or in the file.</p>
<p>This paragraph text would be black unless another style is set on the page or in a file.
```

## Linking to external files

Include styles defined in an external file by adding a link tag within the head of your page as shown below.

```markup
<head>
<link rel="stylesheet" type="text/css" href="css/site.css">
</head>
```

## Your Assignment

1. Copy your style sheet to a separate file. Save it under the WebContent folder in another folder called 'css'. Name your file 'site.css'. Replace the styles in you head tag with a link tag to tell the browser to get the styles from an external file. 
2. Change the color of the first paragraph to blue.

