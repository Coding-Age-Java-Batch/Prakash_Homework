class parents {
void A(){
System.out.println("Parents constructor called");
}

}

class child extends parents{
void B(){
System.out.println("Child constructor called");

     }

     public static void main (String []args){
         child c = new child();
         c.B();
         c.A();
     }
}