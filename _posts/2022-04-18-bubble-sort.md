---
published: true
categories:
  - Array
tags:
  - Array
  - Bubble Sort
  - Sorting
---
## Java program to perform Bubble Sort

> The idea of bubble sort is to move the largest element to the highest index position in the array.
>
> To attain this, two adjacent elements are compared repeatedly and exchanged if they are not in correct order.

```java
public class Main {
    public static void main(String[] args) {
        int a[] = {3, 5, 1, 7, 9, 4};
        
        for(int i = 0; i < a.length-1; i++) {
            for (int j = 0; j < a.length-i-1; j++) {
                if (a[j] > a[j+1]) {
                    int temp = a[j];
                    a[j] = a[j+1];
                    a[j+1] = temp;
                }
            }
        }
        
        for(int i = 0; i < a.length; i++) {
            System.out.print(a[i] + " ");
        }
    }
}
```
