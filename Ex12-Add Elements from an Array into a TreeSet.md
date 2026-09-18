# Ex12 Add Elements from an Array into a TreeSet

## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.

## Algorithm

Create an array containing a few integer elements.

Create a TreeSet to store elements in sorted order.

Use a loop to add each element of the array into the TreeSet.

Display the elements of the TreeSet.

Stop the Program.

## Program:
```
/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: KIRUTHIGA.B
Register Number: 212224040160
*/

import java.util.*;

public class ArrayToTreeSet {

    public static TreeSet<Integer> convertArrayToTreeSet(int[] arr) {
        List<Integer> list = new ArrayList<>();
        for(int x : arr){
            list.add(x);
        }
        
        TreeSet<Integer> treeSet = new TreeSet<>(list);
        return treeSet;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        TreeSet<Integer> treeSet = convertArrayToTreeSet(arr);
        System.out.println("Elements in TreeSet:");
        for (int num : treeSet) {
            System.out.println(num);
        }

        sc.close();
    }
}

```

## Output:

<img width="690" height="480" alt="image" src="https://github.com/user-attachments/assets/c18510dc-4e94-4186-be07-15374c4cfdc2" />




## Result:
The program successfully adds elements from an array into a TreeSet.
