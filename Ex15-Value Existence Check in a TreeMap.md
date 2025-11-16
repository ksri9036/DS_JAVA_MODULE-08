# Ex15 Value Existence Check in a TreeMap
## DATE:16-11-25
## AIM:
To write a Java program that checks whether a given value exists in a TreeMap.

## Algorithm
1. Create a TreeMap<Integer, String> to store key–value pairs in sorted order.

2.Ask the user how many entries they want to insert into the TreeMap.

3.Read keys and values from the user and insert them into the TreeMap.

4.Ask the user for the value they want to search.

5.Use containsValue() to check if the value exists and display the result.
 

## Program:
```
/*
Program to checks whether a given value exists in a TreeMap.
Developed by: Starbiya S
RegisterNumber: 212223040208
*/
import java.util.*;

public class TreeMapValueSearch {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Step 1: Create a TreeMap
        TreeMap<Integer, String> map = new TreeMap<>();

        System.out.print("Enter number of entries: ");
        int n = sc.nextInt();
        sc.nextLine(); // consume newline

        // Step 2 & 3: Take key-value pairs from user
        for (int i = 0; i < n; i++) {
            System.out.print("Enter key (integer): ");
            int key = sc.nextInt();
            sc.nextLine();

            System.out.print("Enter value (string): ");
            String value = sc.nextLine();

            map.put(key, value);
        }

        // Step 4: Ask value to search
        System.out.print("\nEnter value to search: ");
        String searchValue = sc.nextLine();

        // Step 5: Check value exists
        if (map.containsValue(searchValue)) {
            System.out.println("Value \"" + searchValue + "\" exists in the TreeMap.");
        } else {
            System.out.println("Value \"" + searchValue + "\" does NOT exist in the TreeMap.");
        }

        sc.close();
    }
}

```

## Output:

<img width="477" height="322" alt="image" src="https://github.com/user-attachments/assets/cc09c884-a0b1-4adb-955e-2580e3a3c2c8" />


## Result:
Thus, the program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.
