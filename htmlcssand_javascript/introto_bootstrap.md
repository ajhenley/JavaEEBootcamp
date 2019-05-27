# Intro to Bootstrap

Developers like yourself create code. Designers make the interface look nice. But not every project has a designer. Sometimes that job is also yours. Congratulations!

You have a secret weapon. Bootstrap is the most popular HTML, CSS, and JS framework for developing responsive, mobile first projects on the web. Bootstrap is a framework. It uses html, cascading style sheets and JavaScript. Bootstrap contains design templates for typography, forms, buttons, navigation and other interface components.

Bootstrap allows you to create responsive web pages. Responsive web pages adapt their layout to different devices. Without responsive design you would develop different pages for different devices. Bootstrap solves that problem and ends the madness.

The place to get started for Bootstrap is `http://getbootstrap.com/`. If you have any questions about Bootstrap try that site first.

## Including Bootstrap in your JSP or HTML Page

You can download the Bootstrap libraries to your computer and link to them. Or, you could take the easy route and link to a hosted version at a Content Delivery Network. We'll link to the hosted version. Include three links in your web page as shown below. Place the links just before the ending `</head>` tag.

 \#\#\#\#A basic Bootstrap page To create a basic Bootstrap page {%ace edit=false, lang='html'%}Bootstrap 101 Template  {%endace%} Next, add a navigation bar to your page. Put it right below the body tag. Now users of your website won't get lost. {%ace edit=false, lang='html'%}  Toggle navigation [Home](http://mikspot.com/)

```text
    <div class="navbar-collapse collapse">
        <ul class="nav navbar-nav">
            <li class="active">
                <a href="#">All</a>
            </li>
            <li>
                <a href="#">Demo</a>
            </li>
            <li>
                <a href="#">Contact</a>
            </li>
        </ul>
    </div><!--/.nav-collapse -->

</div>
```

&lt;/div&gt;

You need a another `<div>` tag below the navigation bar to denote the page container. The container class sets the content's margins. This keeps the content together as screen size changes. The container class creates 'boxed' contents of your Bootstrap page.

Note: You don't want a container inside a container since nesting containers is not the goal. Having multiple containers is fine. You may wish to wrap the entire contents inside one container. Suit yourself.

Add a Heading. But not just any heading. We're going to create a Jumbotron heading. Let them know we're here!

