# Ex13 Fill the First 10 Elements of an Array with a Constant using Arrays.fill()
## DATE:16-11-25
## AIM:
To write a Java program that fills the first 10 elements of an array with a constant value using the Arrays.fill() method.
## Algorithm
1. Create an integer array of desired size.

2.Choose the constant value to fill.

3.Use Arrays.fill(array, startIndex, endIndex, value) to fill the first 10 elements.

4.Traverse the array (optional) to verify or display elements.

5.Print the array contents.
   

## Program:
```
/*
Program to FILL the first 10 elements of an array with a constant value using the Arrays.fill() method.
Developed by: Starbiya S
RegisterNumber:  212223040208
*/
import java.util.Arrays;

public class FillArrayExample {
    public static void main(String[] args) {

        // Create an array of size 15
        int[] arr = new int[15];

        // Constant value to fill
        int value = 7;

        // Fill first 10 elements with the value
        Arrays.fill(arr, 0, 10, value);  // from index 0 to 9

        // Display the array
        System.out.println("Array after filling first 10 elements: " + Arrays.toString(arr));
    }
}

```

## Output:

<img width="821" height="98" alt="image" src="https://github.com/user-attachments/assets/d1e8a988-a882-46d5-a424-f2771b4b9141" />


## Result:
The program successfully fills the first 10 elements of the array with the constant value 5 using the Arrays.fill() method.
