# Ex11 Convert HashSet to ArrayList in Java

## AIM:
To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.

## Algorithm

Start the program.

Create a HashSet to store a collection of distinct integers.

Add a few integers to the HashSet.

Create an ArrayList and initialize it with the elements of the HashSet.

Display the elements of both HashSet and ArrayList and End the program.


## Program:
```
/*
Program to To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
Developed by: KIRUTHIGA.B
Register Number: 212224040160
*/

import java.util.*;

public class HashSetToArrayList {

    public static ArrayList<Integer> convertToArrayList(HashSet<Integer> set) {
        ArrayList<Integer> list = new ArrayList<>(set);
        return list;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        HashSet<Integer> set = new HashSet<>();
        for (int i = 0; i < n; i++) {
            int num = sc.nextInt();
            set.add(num);
        }

        ArrayList<Integer> list = convertToArrayList(set);
        System.out.println("ArrayList contents:");
        for (int num : list) {
            System.out.print(num + " ");
        }
        sc.close();
    }
}

```

## Output:

<img width="577" height="601" alt="image" src="https://github.com/user-attachments/assets/45f556ae-4eec-49d9-aebf-60a9ed7a51f4" />




## Result:
The program successfully converts a collection of distinct integers stored in a HashSet into an ArrayList
