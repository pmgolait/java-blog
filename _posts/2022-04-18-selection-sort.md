---
published: true
categories:
  - Array
tags:
  - Array
  - Selection Sort
  - Sorting
---
## Java program to perform Selection Sort

> In this method, the next smallest (or next largest) element is found in the array and is moved to its correct position. 

```java
public class Main {
    public static void main(String[] args) {
        int a[] = {3, 5, 1, 7, 9, 4};
        
        for(int i = 0; i <= a.length-1; i++) {
            int smallest = i;
            for(int j = i+1; j < a.length; j++) {
                if(a[smallest]>a[j]){
                    smallest = j;
                }
            }
            int temp = a[smallest];
			a[smallest] = a[i];
  			a[i] = temp;
        }
                                 
		for (int i = 0; i < a.length; i++) {
            System.out.print(a[i] + " ");
        }
    }
}
```
