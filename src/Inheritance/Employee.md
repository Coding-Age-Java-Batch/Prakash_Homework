class Employee {

String Name = "Karan";

    void dispalyInfo(){
        System.out.println("Name :"+ Name);
    }
}

class Manager extends Employee{

    String Department = "HR";


    void disaplayInfo(){
        System.out.println("Department:" + Department);
    }

    public static void main(String[]args){
        Manager m = new Manager();

        m.disaplayInfo();
    }
}
