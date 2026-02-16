public class AreaCalculator {

    int area(int radius){
        return 27/7* radius* radius;
    }

    int area(int length , int breadth){

        return length*breadth;
    }

    double area(double base , double height){
        return 0.5 *base*height;
    }

    public static void main(String[]args){

        AreaCalculator ac= new AreaCalculator();

        System.out.println("Area of circle:"+ ac.area(5));
        System.out.println("Area of rectangle: "+ac.area(4 ,5));
        System.out.println("Area of triangle:"+ ac.area( 6.0 , 4.0));
    }

}
