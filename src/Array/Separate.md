class Separate {
public static void main(String[] args) {
int[] arr = {1,-1,3,-2,5};
int left = 0, right = arr.length - 1;

        while (left <= right) {
            if (arr[left] < 0) {
                left++;
            } else if (arr[right] > 0) {
                right--;
            } else {
                int temp = arr[left];
                arr[left] = arr[right];
                arr[right] = temp;
            }
        }

        for (int num : arr)
            System.out.print(num + " ");
    }
}
