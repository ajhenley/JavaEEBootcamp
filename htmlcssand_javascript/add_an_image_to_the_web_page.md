# HTML5 Attributes with Images

* HTML elements consist of a start tag and an end tag. Often there is content in between the tags,  `<tagname>content</tagname>`.
* Use lower case for element names, attributes and other HTML markup
* The HTML element is everything from the start tag to the end tag, `<p>My first HTML paragraph.</p>`

## HTML5 Attributes:

* Elements may have one or more attributes
* Attributes provide further information about an element
* Attributes are a name-value pair and the value must be in quotes
* There should be no space on either side of the equal sign for attributes
* Attributes are always specified in the start tag. Put them in the end tag? Then I don't know you.

## Add a linked image and some attributes to the Web Page

Images can make your page more interesting and your content more clear. Let's add an image of a crab or crab cake to the new crab cake recipe recipe.

First, find an image. You can use Google images, take one with your camera or copy the link here from Wikipedia.

`https://upload.wikimedia.org/wikipedia/commons/9/99/The_Childrens_Museum_of_Indianapolis_-_Atlantic_blue_crab.jpg`.

To add an image to your page you need an image tag: `<img> ... </img>`. The image tag takes four attributes you need to know about.

`<img src="https://upload.wikimedia.org/wikipedia/commons/9/99/The_Childrens_Museum_of_Indianapolis_-_Atlantic_blue_crab.jpg" alt="Blue Crab before becomming dinner" height="42" width="42">`. Note that the height and width are in pixels.

You could also save the image locally and link to the version on your file system.

## Make the image clickable

Your image could link to another page. Let's make it link to the Wikipedia article from which we took the image. Surround the image with an anchor tag and set the `href` property to the other page. `<a href=""><img ... </img></a>`.

## Your Assignment

Add the crab image to your crab cake recipe page. Change the size settings to your liking. Make the image click through to the wikipedia article at [https://en.wikipedia.org/wiki/Crab\_cake](https://en.wikipedia.org/wiki/Crab_cake). Now when you click on the image you'll be redirected.

Add another attribute to your anchor tag. It should be called target and the value should be "\_blank": `target="_blank"`. How does that change your page?

