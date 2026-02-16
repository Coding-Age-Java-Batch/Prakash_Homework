class person {

     void showDetails(){
         System.out.println("Person Details ");
     }
}

class Students extends person {

     @Override
     void showDetails(){
         System.out.println("Students Details");
     }

     public static void main (String[]args){
         Students s = new Students();
         s.showDetails();
     }

}
