class single {
void show(){
System.out.println("single ");

     }
}

class single2 extends single{

     @Override
     void show(){
         System.out.println("singl2");
     }

     public static void main(String[]args){

         single2 s = new single2();
         s.show();
     }
}
