class MissingNumber {
public static void main(String[] args) {
int[] arr = {1, 2, 4, 5};
int n = 5;

        int a = n * (n + 1) / 2;
        int b = 0;

        for (int num : arr) {
            b += num;
        }

        System.out.println("Missing Number = " + (a - b));
    }
}
