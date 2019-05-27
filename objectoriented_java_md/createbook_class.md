# Create book class

Congratulations. For your next assignment, you'll develop an application to manage an inventory of books.

Create a new project in Eclipse called BookApplication. Right-click on your project and add a class.

Create a Book class that allows for the following fields:

* SKU \(stockkeeping unit - will serve as unique ID for each book\)
* Book title
* Author
* Description
* Price
* IsInStock

You'll start by creating a project in Eclipse called BookApplication.

Your book application will need a class. Create a class and name it Book. All classes in Java begin with a capital letter.

Next, you'll add private member variables for each field above. You can't have spaces so name them accordingly. The first private member variable would probably be `private String bookTitle`

Next, you'll create getters and setters for each field. The getters and setters for bookTitle would look like this:

```java
public class Book {
    private String bookTitle;

    public String getBookTitle() {
        return bookTitle;
    }

    public void setBookTitle(String bookTitle) {
        this.bookTitle = bookTitle;
    }
}
```

Notice that your Book class will not contain a method called main. That's because main is in a different part of your program. You'll see that in the upcoming assignment to create a book app.

Main will call the Book class to create an object of type Book. Then we can populate the title by calling the setter and passing the bookTitle as a String.

```java
public class BookApplication {

    public static void main(String[] args) {

        Book myBook = new Book();
        myBook.setBookTitle("This Book Needs a Title");

    }
}
```

Create a method that returns the pricing for a requested number of books. Five books at $20.00 should return $100, if they are in stock. If they are not in stock, you should return an appropriate value.

Finally, create a constructor for your class. The constructor is a method that can be used to initialize your variables. The constructor always has the same name as the class. When an object is instantiated using the keyword 'new' the constructor will always be called. Set each private member variable to an appropriate initial value. That would be an empty string for text, 0 for integers and 0.0 for other numeric values.

