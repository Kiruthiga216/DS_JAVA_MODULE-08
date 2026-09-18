# Ex13 Fill the First 10 Elements of an Array with a Constant using Arrays.fill()

## AIM:
To write a Java program that fills the first 10 elements of an array with a constant value using the Arrays.fill() method.

## Algorithm

Start the program.

Create an integer array of a specified size (for example, 15 elements).

Use the Arrays.fill() method to fill the first 10 elements of the array with a constant value

Display the elements of the array after filling.

Stop the program.

 

## Program:
```
/*
Program to FILL the first 10 elements of an array with a constant value using the Arrays.fill() method.
Developed by: KIRUTHIGA.B
Register Number: 212224040160
*/

import java.util.*;

public class FillArrayUsingArraysFill {

    public static int[] fillArray(int size, int value) {
        int[] arr = new int[size];
        Arrays.fill(arr, value);
        return arr;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int value = sc.nextInt();
        int[] arr = fillArray(10, value);
        System.out.println("Array elements:");
        for (int num : arr) {
            System.out.print(num + " ");
        }
        sc.close();
    }
}

```

## Output:

<img width="772" height="190" alt="image" src="https://github.com/user-attachments/assets/e9e32070-b65e-4353-bf16-435610fd95f1" />




## Result:
The program successfully fills the first 10 elements of the array with the constant value 5 using the Arrays.fill() method.
