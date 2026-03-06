interface Operation {
int operate(int a, int b);
}

public class TestOperation {
public static void main(String[] args) {

        Operation add = new Operation() {
            public int operate(int a,int b){ return a+b; }
        };

        Operation sub = new Operation() {
            public int operate(int a,int b){ return a-b; }
        };

        Operation mul = new Operation() {
            public int operate(int a,int b){ return a*b; }
        };

        Operation div = new Operation() {
            public int operate(int a,int b){ return a/b; }
        };

        System.out.println(add.operate(10,5));
        System.out.println(sub.operate(10,5));
        System.out.println(mul.operate(10,5));
        System.out.println(div.operate(10,5));
    }
}