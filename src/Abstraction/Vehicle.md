abstract class Vehicle {
String brand;
private int speed;

    abstract void drive();

    public void setSpeed(int speed) {
        if (speed <= 300) this.speed = speed;
        else System.out.println("Error: Speed exceeds limit!");
    }
    public int getSpeed() { 
    return speed;
    }
}

class Car extends Vehicle {
void drive() { 
System.out.println(brand + " car is driving at " + getSpeed() + " km/h"); 
}
}