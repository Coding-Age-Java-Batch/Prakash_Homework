public class Greeter {

    void greet(){
        System.out.println("Hello!");
    }

    void greet(String name){

        System.out.println("Hello " + name +"!");

    }

    void greet(String name , String timeofday){
        System.out.println("Good "+ timeofday +","+name+"!");
    }

    public static void main(String[]args){
        Greeter g = new Greeter();
        g.greet();
        g.greet("Riya");
        g.greet("Riya", " M0rning");
    }
}
