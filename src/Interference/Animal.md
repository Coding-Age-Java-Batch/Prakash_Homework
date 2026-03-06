interface Animal {
void makeSound();
}

class Dog implements Animal {
public void makeSound() {
System.out.println("Dog: Bark");
}
}

class Cat implements Animal {
public void makeSound() {
System.out.println("Cat: Meow");
}
}

class Cow implements Animal {
public void makeSound() {
System.out.println("Cow: Moo");
}
}

public class TestAnimal {
public static void main(String[] args) {

        Animal[] animals = {
            new Dog(),
            new Cat(),
            new Cow()
        };

        for(Animal a : animals)
            a.makeSound();
    }
}