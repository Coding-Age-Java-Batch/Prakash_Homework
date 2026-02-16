public class Student {

    void printDetails(String name , int age){

        System.out.println("Name:"+name + ",Age:" + age);

    }
    void printDetails(String name, int age , String course){

        System.out.println("Name:"+name + ",Age: "+age +"Course:" + course );
    }

    public static void main(String[]args){

        Student  s = new Student();
        s.printDetails("Rahul", 20);
        s.printDetails("Priya",19, "B.Tech");
    }


}
