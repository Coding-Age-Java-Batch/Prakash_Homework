Class RemoveDuplication {
import java.util.ArrayList;
public static void main(String[] args) {
ArrayList<Integer> list = new ArrayList<>(Arrays.asList(1, 2, 2, 3, 3));

        Set<Integer> set = new LinkedHashSet<>(list);
        ArrayList<Integer> uniqueList = new ArrayList<>(set);

        System.out.println(uniqueList);
    }
}
