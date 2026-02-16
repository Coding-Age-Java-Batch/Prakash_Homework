class Book {

    String title = "Java Basics";
    String author = "John smith";

    void showdetails(){

        System.out.println("Title: "+ title);
        System.out.println("Author: "+ author);
    }
}

class Libarybook extends Book{

    int Shelfnumber = 5 ;

    @Override
    void showdetails(){

        System.out.println("Shelfnumber: " + Shelfnumber);

    }

    public static void main(String[]args){
        Libarybook lb = new Libarybook();

        lb.showdetails();
    }
}
