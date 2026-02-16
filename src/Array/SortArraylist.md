class SortArrayList {
import java.util.ArrayList;
import java.util.Collections;
public static void main(String[] args) {
ArrayList<Integer> list = new ArrayList<>();
list.add(4);
list.add(1);
list.add(3);
list.add(2);

        Collections.sort(list);
        System.out.println(list);
    }
}
