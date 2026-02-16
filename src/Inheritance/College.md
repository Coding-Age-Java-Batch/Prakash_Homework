class College {

    String collegeName = "Techno  Institute";

    void display(){
        System.out.println("College: "+ collegeName);
    }
}

class Admission extends College{

    String studentName = "Ananya";
    String course = "B.Tech";

    @Override
    void display() {
        System.out.println("Student:"+ studentName);
        System.out.println("course:"+ course);
    }

    public static void main(String[]args){

        Admission a = new Admission();

        a.display();
    }
}
