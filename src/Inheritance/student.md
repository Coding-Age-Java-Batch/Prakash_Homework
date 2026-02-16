class Student {
String Name = "Ravi";

     void display(){

         System.out.println("Name: "+ Name);
     }

}

class marksheet extends Student{

    int science = 80 ;
    int maths = 95;
    int computer = 95;

    @Override
    void display() {
        System.out.println("total :" + (science + maths + computer));
    }

    public static void main(String[]args){

        Student s= new Student();
        s.display();
        marksheet ma = new marksheet();
        ma.display();

    }

}
