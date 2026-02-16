public class student {
String Name;
int Rollno;
double Marks;

    void setDetails(String name , int rollno, double marks){

        Name = name;
        Rollno = rollno;
        Marks = marks;
    }

    void displayInfo() {
        System.out.println("Name:" +Name);
        System.out.println("Rollno:" +Rollno);
        System.out.println("Marks:" +Marks);
    }

    void hasPassed(){
        if (Marks>=40){
            System.out.println("true");
        }
        else {
            System.out.println("false");
        }
    }

    public static void main(String[]args){
        student s =new student();

        s.setDetails("prakash kumar", 23 , 98.8);
        s.displayInfo();
        s.hasPassed();

    }

}

