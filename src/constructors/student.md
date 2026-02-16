public class Student {
int StudentId;
String StudentName;

    public Student(int id , String name ){
        StudentId= id;
        StudentName = name;
    }

public void StudentInPrinter(){

        System.out.println("Student ID:" + StudentId);
        System.out.println("Student Name " + StudentName);

    }

    public static void main(String[]args){

        Student s = new Student( 10 , "Prakash Kumar");
        s. StudentInPrinter();

    }

}
