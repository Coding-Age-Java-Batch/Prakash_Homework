interface Taxable {
double calculateTax(double income);
}

class Employee implements Taxable {
public double calculateTax(double income) {
return income * 0.10;
}
}

class Business implements Taxable {
public double calculateTax(double income) {
return income * 0.15;
}
}