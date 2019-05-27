# Create book app

A book app will allow the user to retrieve an instance of a book. Here's a start. To retrieve a particular book you'll need to set the SKU to an existing SKU.

Next: Add some code to display the title and author of the book to the console.

What happens if you try to retrieve a SKU that doesn't exist?

```java
public class BookApplication {

    public static void main(String[] args) {

        String bookSKU = "Zombie1005";
        Book myBook = new Book();
        myBook.setSKU(bookSKU);
    }
}
```

