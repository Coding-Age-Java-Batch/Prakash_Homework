public class book {

    String Title;
    String Author;
    int Price;

    public book (String title , String author , int price){
        Title = title;
        Author = author;
        Price = price;
    }

    public book (String title , String author){
        Title = title;
        Author = author;
    }

    public void displayDetails(){
        System.out.println("Title: " + Title);
        System.out.println("Author: " + Author);
        System.out.println("Price: " + 250);
    }


    public static void main(String[]args){

        book b = new book("Java Essentials", "John Doe");
        b.displayDetails();
    }


}
