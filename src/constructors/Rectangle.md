class Rectangle {
double length;
double breadth;

    Rectangle(double length, double breadth) {
        this.length = length;
        this.breadth = breadth;
    }

    boolean hasEqualArea(Rectangle other) {
        double area1 = this.length * this.breadth;
        double area2 = other.length * other.breadth;
        return area1 == area2;
    }

    public static void main(String[] args) {
        Rectangle r1 = new Rectangle(10, 5);
        Rectangle r2 = new Rectangle(25, 2);

        boolean result = r1.hasEqualArea(r2);
        System.out.println("Rectangle 1 and Rectangle 2 have equal area: " + result);
    }
}
