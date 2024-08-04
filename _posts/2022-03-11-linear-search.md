---
published: true
categories:
  - Array
tags:
  - Array
  - Linear Search
  - Searching
---
## Java Program to perform Linear Search

> Linear Search refers to the searching technique in which each element of an array is compared with the search item, one by one, until the search-item is found or all elements have been compared.

```java
public class Main {
    public static void main (int n) {
        int[] a = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
        int flag = 0, i;
        
        for (i = 0; i < a.length; i++) {
            if (n==a[i]) {
                flag++;
                break;
            }
	}
        
        if(flag!=0){
            System.out.println("element found at : " + (i+1));
        }
        else {
            System.out.println("element not found!");
        }
    }
}
```
