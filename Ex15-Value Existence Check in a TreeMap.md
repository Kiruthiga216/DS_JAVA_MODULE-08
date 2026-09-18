# Ex15 Value Existence Check in a TreeMap

## AIM:
To write a Java program that checks whether a given value exists in a TreeMap.

## Algorithm

Create a TreeMap to store key–value pairs.

Insert some sample key–value pairs into the TreeMap.

Display the contents of the TreeMap.

Use the containsValue() method to check whether a specific value exists in the map

Display the result based on the check.

## Program:
```
/*
Program to checks whether a given value exists in a TreeMap.
Developed bY: KIRUTHIGA.B
Register Number: 212224040160
*/

import java.util.*;

public class TreeMapValueExistenceCheck {

    public static void checkValue(TreeMap<Integer, String> map, String searchValue) {
        if(map.containsValue(searchValue)){
            System.out.println("Value \""+searchValue+"\" exists in the TreeMap.");
        }else{
            System.out.println("Value \""+searchValue+"\" does not exist in the TreeMap.");
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        TreeMap<Integer, String> map = new TreeMap<>();

        int n = sc.nextInt();

        for (int i = 0; i < n; i++) {
            int key = sc.nextInt();
            sc.nextLine();  
            String value = sc.nextLine();
            map.put(key, value);
        }
        String searchValue = sc.nextLine();

        checkValue(map, searchValue);
        sc.close();
    }
}

```

## Output:

<img width="815" height="556" alt="image" src="https://github.com/user-attachments/assets/04429bb2-5b85-4eff-9b07-f70f83a2153c" />




## Result:
Thus, the program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.
