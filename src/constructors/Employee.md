public class Employee{
int Id;
String Name;
String Department;

    public Employee(int id , String name , String department){
        Id = id;
        Name = name;
        Department = department;

    }

    public Employee(int id, String name) {
        Id = id;
        Name = name;


    }

    public void displayDetails(){
        System.out.println("Id:" + Id);
        System.out.println("Name:" + Name);
        System.out.println("Department:" + Department);
    }

    public static void main(String[]args){
        Employee emp = new Employee(101 , "Alice");
        emp.displayDetails();

    }


}
