# Ex11 Convert HashSet to ArrayList in Java
## DATE: 16-11-25
## AIM:
To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
## Algorithm
1.Start and create an empty HashSet.

2.Insert all the required integers into the HashSet.

3.Create an ArrayList and pass the HashSet to its constructor.

4.Store all elements of the HashSet into the ArrayList.

5.Display the elements of the ArrayList.
 

## Program:
```
/*
Program to To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
Developed by: Starbiya S
RegisterNumber:  212223040208
*/
import java.util.*;

public class HashSetToArrayList {
    public static void main(String[] args) {

        // Create a HashSet of integers
        HashSet<Integer> numberSet = new HashSet<>();

        Scanner sc = new Scanner(System.in);
        System.out.print("Enter how many numbers you want to add: ");
        int n = sc.nextInt();

        // Taking input from the user
        System.out.println("Enter " + n + " distinct integers:");
        for (int i = 0; i < n; i++) {
            numberSet.add(sc.nextInt());
        }

        // Convert HashSet to ArrayList
        ArrayList<Integer> numberList = new ArrayList<>(numberSet);

        // Display the ArrayList
        System.out.println("\nArrayList contents:");
        for (int num : numberList) {
            System.out.println(num);
        }

        sc.close();
    }
}

```

## Output:

<img width="678" height="428" alt="image" src="https://github.com/user-attachments/assets/7ad8f4e2-b4ec-4332-b85e-58261bdbfbeb" />


## Result:
The program successfully converts a collection of distinct integers stored in a HashSet into an ArrayList

# Ex12 Add Elements from an Array into a TreeSet
## DATE:16-11-25
## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
1.Start and create an integer array.

2.Create an empty TreeSet.

3.Traverse the array using a loop.

4.Insert each array element into the TreeSet.

5.Display the TreeSet (elements appear in sorted order automatically). 
  

## Program:
```
/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: Starbiya S
RegisterNumber: 212223040208 
*/
import java.util.*;

public class ArrayToTreeSet {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        // Take array size from user
        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();

        int[] arr = new int[n];

        // Input array elements
        System.out.println("Enter " + n + " integers:");
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        // Create a TreeSet
        TreeSet<Integer> set = new TreeSet<>();

        // Add array elements to TreeSet
        for (int num : arr) {
            set.add(num);
        }

        // Display sorted elements
        System.out.println("Elements in sorted order (TreeSet): " + set);

        sc.close();
    }
}

```

## Output:
<img width="620" height="280" alt="image" src="https://github.com/user-attachments/assets/d6bd387c-0acc-465f-ac38-9b7f3f38e35c" />



## Result:
The program successfully adds elements from an array into a TreeSet.

