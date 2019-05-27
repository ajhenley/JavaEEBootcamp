# Explore the DOM with JavaScript

![](https://upload.wikimedia.org/wikipedia/commons/8/8b/Simpe_HTML_page_DOM.svg)

JavaScript can access and change all the elements of an HTML document. With that power you can make your web page dynamic. The HTML DOM is a standard for how to get, change, add, or delete HTML elements.

## What is the DOM?

The browser creates a Document Object Model of your web page. The DOM model is a tree of Objects. It defines:

* The HTML elements as objects
* The properties of all HTML elements
* The methods to access all HTML elements
* The events for all HTML elements

Add the following script between the `<head> ... </head>` tags of the last web page you created. When you click on the button the script will list all the elements in the DOM for your web page. Add elements to your page and run the script again. You will see the new elements listed.

```markup
<script>
<!--
function listTags()
{
 var tag, tags;
 // or you can use var allElem=document.all; and loop on it
 tags = "The tags in the page are:"
 for(i = 0; i < document.all.length; i++)
 {
   tag = document.all(i).tagName;
   tags = tags + "<br/>" + tag;
 }
 document.write(tags);
}// -->
</script>


Also, add the following button to your page so the function will run when the user clicks the button.

```html
<button onclick="listTags()">List my Tags</button>
```

