public class Shape {

    void printShape(){
        System.out.println("This is a shape");
    }

    void printShape(String square , String triangle){
        System.out.println("This is  a square");
        System.out.println("This is a triangle");
    }


    public static void main(String[]args){

        Shape s = new Shape();

        s.printShape();
        s.printShape(",", ",");
    }
}
