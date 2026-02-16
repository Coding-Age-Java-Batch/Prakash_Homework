class Food {

     String foodName = "Gulab  Jamun";

     void display(){

         System.out.println("Food :" +foodName);
     }
}

class Dessert extends Food{

     String sweetnessLevel = "High";


    @Override
    void display() {
        System.out.println("Level: "+ sweetnessLevel);

    }

    public static void main(String[]args){

        Dessert d = new Dessert();
        d.display();
    }
}
