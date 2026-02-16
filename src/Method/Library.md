public class Library {

    String Title;
    String Author;
    boolean IsAvailable;

    void setDetails(String title, String author){
        Title = title;
        Author = author;
        IsAvailable = true ;

    }

    void borrowBook(){
        if (IsAvailable){
            IsAvailable = false;
            System.out.println("Marks isAvailable" +IsAvailable );
        }

    }

    void returnBOOK(){
        if (IsAvailable){
            IsAvailable = true;
            System.out.println("Marks isAvailable" + IsAvailable);
        }
        
    }
    void dispalyStatus(){
        System.out.println("Title:" +Title);
        System.out.println("Author" +Author);
        System.out.println("IsAvailable" +IsAvailable);
    }


    public static void main(String[]args) {
        Library l = new Library();
        l.setDetails( "p.k" , "Prakash");
        l.borrowBook();
        l.returnBOOK();
        l.dispalyStatus();
    }
}
