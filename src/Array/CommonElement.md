class CommonElement {
import java.util.CommomElement;
public static void main(String[] args) {
ArrayList<Integer> A = new ArrayList<>(Arrays.asList(1,2,3));
ArrayList<Integer> B = new ArrayList<>(Arrays.asList(2,3,4));

        A.retainAll(B);
        System.out.println(A);
    }
}
