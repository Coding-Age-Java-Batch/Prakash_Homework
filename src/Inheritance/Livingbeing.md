class Livingbeing {
void breath(){
System.out.println("Breathing");

    }
}

class animal extends Livingbeing {
void eat(){
System.out.println("Eating");
}
}
class dog extends animal{
void bark(){

        System.out.println("Barking");

    }

    public static void main( String[]args) {

        dog h = new dog();
         h.bark();
         h.eat();
         h.breath();

    }


}
