# MVC: Model View Controller

A commonly used software architectural pattern, MVC divides an application into three interconnected parts.

Keeping these three components separate ensures each one is independent of the others. Changes made to one will not affect changes to the others. The web interface can be updated with a new look without impacting the database or the business rules in the controller.

![](https://upload.wikimedia.org/wikipedia/commons/a/a0/MVC-Process.svg)

## Components

**The model** directly manages the data, logic and rules of the application. The model is represented in your application by Oracle and any data-management related classes.

**A view** can be any output representation of information, such as a chart or a diagram. Multiple views of the same information are possible. For example, you might show a bar chart to management and a tabular view to accountants. The web page in the browser represents the view in applications created for this course.

**The controller** accepts input and converts it to commands for the model or view. The controller can also manage the logic and rules of the application. The servlet represents the controller in applications created for this course.

## Interactions between the components

* A controller sends commands to the model. These commands can update the model's state \(e.g. editing a document\). The controller also sends commands to its associated view. This changes the view's presentation of the model.
* A model stores the data. Commands from the controller retrieve the data and display it in the view.
* A view generates an output presentation to the user based on changes in the model.

## How this affects you

When you develop an application you'll create a database. The model will represent the database. Secondly you'll develop a page for the user. This is the view, also called the presentation. Finally, you'll code some business rules that the client wants the application to enforce. These go into the controller along with code help the view interact with the model.

