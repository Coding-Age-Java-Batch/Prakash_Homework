public class Calculator {

    static int add(int a , int b){
        return a + b;

    }

    static int subtract(int a , int b ){
        return a - b ;

    }

    static int multiply(int a, int b){
        return a * b;
    }

    static int divide(int a , int b){
        return a / b;
    }

    public static void main(String[]args){
        int sum = add(5 , 9);
         System.out.println("Sum = " + sum);
         int difference = subtract(67 , 46);
         System.out.println("Difference =" + difference);
         int product = multiply(9 ,7);
         System.out.println("Product =" + product);
         int quotientn = divide(25 , 5);
         System.out.println("Quotient =" + quotientn);
    }
}

