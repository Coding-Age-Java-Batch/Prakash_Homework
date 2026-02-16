public class Calculator {

    int  add(int a , int b){
        return a+b ;
    }

    void result1(){

        System.out.println("result1:"+ add(10,20));
    }

    int add(int a, int b , int c){
        return a+b+c;
    }

    void result2(){

        System.out.println("result2:"+ add(5,10,15));
    }

    public static void main(String[]args){

        Calculator c = new Calculator();

        c.result1();
        c.result2();



    }


}
