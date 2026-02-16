class Shape {
void area(){
System.out.println("Calculating area");
}
}

class Rectangle extends Shape{
int length = 10;
int breadth = 5;
void area(){
System.out.println("Area of Rectangle :" +(length*breadth));

     }

     public static void main(String[]args){
         Rectangle r = new Rectangle();
         r.area();
     }
}

