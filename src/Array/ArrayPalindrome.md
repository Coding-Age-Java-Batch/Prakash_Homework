class ArrayPalindrome {
public static void main(String[] args) {
int[] arr = {1, 2, 3, 2, 1};
boolean isPalindrome = true;

        int start = 0;
        int end = arr.length - 1;

        while (start < end) {
            if (arr[start] != arr[end]) {
                isPalindrome = false;
                break;
            }
            start++;
            end--;
        }

        System.out.println(isPalindrome);
    }
}