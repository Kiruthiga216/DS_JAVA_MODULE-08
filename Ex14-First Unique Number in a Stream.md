# Ex14 Tracking the First Unique Number in a Stream using LinkedHashMap

## AIM:
To implement a program that tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.

## Algorithm

Start the program.

Create a LinkedHashMap to store integers as keys and their frequency (count) as values.

Read or define a stream of integers (array of numbers).

For each integer in the stream:

If the number is not already in the map, insert it with count = 1.

If it exists, increment its count by 1.

After processing each element, find the first number in the LinkedHashMap with count = 1 (the first unique number).

Display the current stream and the first unique number.
   

## Program:
```
/*
Program to tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.
Developed by: KIRUTHIGA.B
Register Number: 212224040160
*/

import java.util.*;

public class FirstUniqueNumberStream {

    public static void processStream(int n, Scanner sc) {
        LinkedHashMap<Integer, Integer> freqMap = new LinkedHashMap<>();
        for(int i=0; i<n; i++){
            int current = sc.nextInt();
            
            freqMap.put(current, freqMap.getOrDefault(current, 0)+1);
            
            int fUniq = -1;
            
            for(Map.Entry<Integer, Integer> entry : freqMap.entrySet()){
                if(entry.getValue() == 1){
                    fUniq = entry.getKey();
                    break;
                }
            }
            
            if(fUniq != -1){
                System.out.println("First unique number: "+fUniq);
            }else{
                System.out.println("No unique number");
            }
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        processStream(n, sc);
        sc.close();
    }
}

```

## Output:

<img width="753" height="558" alt="image" src="https://github.com/user-attachments/assets/863bf41e-00a4-421b-9d22-6f2e1b1aeb81" />




## Result:
The program successfully tracks and returns the first unique number at any point in the integer stream using a LinkedHashMap.
