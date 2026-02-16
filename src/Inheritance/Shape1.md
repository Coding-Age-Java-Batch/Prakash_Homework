public class Shape1 {

    void perimeter(){

        System.out.println("Calculating perimeter");
    }
}

class square extends Shape1{

    int Side = 10;

    @Override
    void perimeter(){

        System.out.println("Perimeter of square :" + (4*Side));
    }

    public static void main (String []args){

        square s = new square();

        s.perimeter();
    }

}