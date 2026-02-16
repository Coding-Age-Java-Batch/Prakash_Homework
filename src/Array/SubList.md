class SubList {
import java.util.SubList;
public static void main(String[] args) {
ArrayList<Integer> list = new ArrayList<>(Arrays.asList(10,20,30,40,50));
List<Integer> sub = list.subList(1,4);

        System.out.println(sub);
    }
}
