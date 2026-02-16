interface Printer {
void print(String document);
}
class InkjetPrinter implements Printer {
public void print(String document) {
System.out.println("Inkjet Printer is printing: " + document);
}
}
class LaserPrinter implements Printer {
public void print(String document) {
System.out.println("Laser Printer is printing: " + document);
}
}
public class Main {
public static void main(String[] args) {

        Printer inkjet = new InkjetPrinter();
        Printer laser = new LaserPrinter();

        inkjet.print("Assignment Document");
        laser.print("Project Report");
    }
}