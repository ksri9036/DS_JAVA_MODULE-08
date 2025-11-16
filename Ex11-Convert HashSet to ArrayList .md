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
