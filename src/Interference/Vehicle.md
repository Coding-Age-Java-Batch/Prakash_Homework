interface Vehicle {
void start();
void stop();
String fuelType();
}

class Car implements Vehicle {
public void start() {
System.out.println("Car started");
}

    public void stop() {
        System.out.println("Car stopped");
    }

    public String fuelType() {
        return "Petrol";
    }
}

class Bike implements Vehicle {
public void start() {
System.out.println("Bike started");
}

    public void stop() {
        System.out.println("Bike stopped");
    }

    public String fuelType() {
        return "Petrol";
    }
}

public class TestVehicle {
public static void main(String[] args) {
Vehicle car = new Car();
Vehicle bike = new Bike();

        car.start();
        System.out.println("Fuel: " + car.fuelType());
        car.stop();

        bike.start();
        System.out.println("Fuel: " + bike.fuelType());
        bike.stop();
    }
}