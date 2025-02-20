# Diffrence-Arrays-ArrayLists
import java.util.ArrayList;

public class DifferenceArraysArrayLists {
    public static void main(String[] args) {
        // Working with Arrays
        int[] numbersArray = new int[3]; // Fixed-size array
        numbersArray[0] = 10;
        numbersArray[1] = 20;
        numbersArray[2] = 30;
        
        System.out.println("Array Elements:");
        for (int num : numbersArray) {
            System.out.print(num + " ");
        }
        System.out.println("\nArray length: " + numbersArray.length);

        // Working with ArrayLists
        ArrayList<Integer> numbersList = new ArrayList<>(); // Dynamic-size list
        numbersList.add(10);
        numbersList.add(20);
        numbersList.add(30);
        numbersList.add(40); // Adding an extra element (not possible in arrays)

        System.out.println("\nArrayList Elements:");
        for (int num : numbersList) {
            System.out.print(num + " ");
        }
        System.out.println("\nArrayList size: " + numbersList.size());

        // Removing an element (only possible in ArrayLists)
        numbersList.remove(2);
        System.out.println("\nArrayList after removing index 2:");
        for (int num : numbersList) {
            System.out.print(num + " ");
        }
        System.out.println("\nUpdated ArrayList size: " + numbersList.size());
    }
}
