class SearchArraylist{
import java.util.Arraylist;
public static void main(String[] args) {
ArrayList<Integer> list = new ArrayList<>();
list.add(10);
list.add(20);
list.add(30);

        int search = 20;

        if (list.contains(search)) {
            System.out.println("Found at index " + list.indexOf(search));
        } else {
            System.out.println("Not Found");
        }
    }
}
