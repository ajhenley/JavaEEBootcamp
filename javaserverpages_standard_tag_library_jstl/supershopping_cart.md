# Super Shopping Cart

This assignment builds on the completed shopping cart application. You should be using JPA and JSTL for this project. You will be creating users, including the Admin user, adding regular users, making your application follow the principles of Model View Controller \(MVC\) and displaying a nice user interface.

## Your Assignment:

* Save the shopping cart to the database. The user should be able to come back and add items to the cart again.
* Allow for multiple users. Each user should only see the items in their shopping cart.
* Your application shall allow a new \(non-admin\) user to register for your site.
* Only registered users can place an order however any user can view products.
* Create an admin user that can see all orders that have been placed.
* Modify your servlet such that the doGet and doPost only call another method, doProcess which does all the work of the servlet. DoProcess should pass as much code as possible to other classes.
* Use the JSTL to display the cart or orders to the JSP pages  you create. Use the foreach tag to loop through and display your cart. 
* You cart must contain a line that says: "You have 1 item in your cart" The 1 should reflect the number of items in the cart  and if there are multiple items then the word items must be plural. Use the JSTL if statement or choose construct to make this work.
* Charge the user a 6% tax. Show the tax on the order confirmation page but not the shopping cart page.
* Allow users to post comments or reviews on the product details page. You must include at least three comments for one product and add comments to three or products. Comments shall include the user's name and date and the number of stars. Search Google images for "Review Stars" or simply use Asterisks.
* Make your JSP smaller by including a header and a footer in every page. You can create the header/footer in a separate JSP page and include it in every page with the following code:
* Use Bootstrap to make your page look nice and contain a navigational bar. Bootstrap should also validate the user's email address and other information that the user enters. You can even put the Bootstrap code in a separate page and include it as shown above.

