// Java Program to Sort the Elements in Descending Order
import java.util.*;

// Driver Class
class GFG {
      // Main Method
    public static void main(String[] args)
    {
        // Initializing the array
        Integer array[] = { 1, 2, 3, 4, 5 };

        // Sorting the array in descending order
        Arrays.sort(array, Collections.reverseOrder());

        // Printing the elements
        System.out.println(Arrays.toString(array));
    }
}



// Java Program to Sort the Elements
// In Descending Order
import java.util.*;

// Driver Class
class GFG {
      // Main Methods
    public static void main(String[] args)
    {
        // Initializing the array
        int array[] = { 1, 2, 3, 4, 5, 6 };

        // Sorting the array in ascending order
        Arrays.sort(array);

        // Reversing the array
        reverse(array);

        // Printing the elements
        System.out.println(Arrays.toString(array));
    }

    public static void reverse(int[] array)
    {
        // Length of the array
        int n = array.length;

        // Swapping the first half elements 
        // With last Half Elements
        for (int i = 0; i < n / 2; i++) {

            // Storing the first half elements temporarily
            int temp = array[i];

            // Assigning the first half
              // to the last half
            array[i] = array[n - i - 1];

            // Assigning the last half
            // to the first half
            array[n - i - 1] = temp;
        }
    }
}
