interface Shape {
double area();
double perimeter();
}

class Circle implements Shape {
double radius;

    Circle(double r) {
        radius = r;
    }

    public double area() {
        return Math.PI * radius * radius;
    }

    public double perimeter() {
        return 2 * Math.PI * radius;
    }
}

class Rectangle implements Shape {
double width, height;

    Rectangle(double w, double h) {
        width = w;
        height = h;
    }

    public double area() {
        return width * height;
    }

    public double perimeter() {
        return 2 * (width + height);
    }
}

class Triangle implements Shape {
double a, b, c;

    Triangle(double a, double b, double c) {
        this.a=a;
        this.b=b;
        this.c=c;
    }

    public double area() {
        double s = (a+b+c)/2;
        return Math.sqrt(s*(s-a)*(s-b)*(s-c));
    }

    public double perimeter() {
        return a+b+c;
    }
}