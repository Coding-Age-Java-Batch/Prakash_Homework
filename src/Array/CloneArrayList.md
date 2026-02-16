class CloneArrayList {
import java.util.ArrayList;
public static void main(String[] args) {
ArrayList<Integer> listA = new ArrayList<>();
listA.add(10);
listA.add(20);

        ArrayList<Integer> listB = new ArrayList<>(listA);

        System.out.println("Cloned List: " + listB);
    }
}
