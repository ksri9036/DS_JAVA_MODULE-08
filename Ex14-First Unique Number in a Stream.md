# Ex14 Tracking the First Unique Number in a Stream using LinkedHashMap
## DATE: 16-11-25
## AIM:
To implement a program that tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.

## Algorithm
1.Create a LinkedHashMap<Integer, Integer> to store each number and its frequency.

2.Read a stream of integers from the user (array or until a certain count).

3.For each number, update its frequency in the LinkedHashMap.

4.Traverse the LinkedHashMap entries in insertion order and find the first entry whose frequency is 1.

5.Display the first unique number. If none exists, print "No unique number". 
  

## Program:
```
/*
Program to tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.
Developed by: Starbiya S 
RegisterNumber: 212223040208 
*/
import java.util.*;

public class FirstUniqueNumber {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Step 1: LinkedHashMap to maintain insertion order + frequency
        LinkedHashMap<Integer, Integer> map = new LinkedHashMap<>();

        System.out.print("Enter number of elements: ");
        int n = scanner.nextInt();

        System.out.println("Enter " + n + " integers:");

        // Step 2 & 3: Take input & update frequency
        for (int i = 0; i < n; i++) {
            int num = scanner.nextInt();
            map.put(num, map.getOrDefault(num, 0) + 1);
        }

        // Step 4: Find first unique number
        Integer firstUnique = null;

        for (Map.Entry<Integer, Integer> entry : map.entrySet()) {
            if (entry.getValue() == 1) {
                firstUnique = entry.getKey();
                break;
            }
        }

        // Step 5: Output the result
        if (firstUnique != null) {
            System.out.println("First unique (non-repeating) number: " + firstUnique);
        } else {
            System.out.println("No unique number exists.");
        }

        scanner.close();
    }
}

```

## Output:

<img width="597" height="345" alt="image" src="https://github.com/user-attachments/assets/f23751b6-70fd-4c9e-b66c-6d4d2a671c8b" />



## Result:
The program successfully tracks and returns the first unique number at any point in the integer stream using a LinkedHashMap.
