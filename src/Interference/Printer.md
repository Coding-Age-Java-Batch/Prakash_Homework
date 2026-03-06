interface Printer {
void print();
}

interface Scanner {
void scan();
}

class MultiFunctionDevice implements Printer, Scanner {

    public void print() {
        System.out.println("Printing Document...");
    }

    public void scan() {
        System.out.println("Scanning Document...");
    }
}

public class TestDevice {
public static void main(String[] args) {
MultiFunctionDevice mfd = new MultiFunctionDevice();
mfd.print();
mfd.scan();
}
}