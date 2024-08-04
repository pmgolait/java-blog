---
published: true
categories:
  - Array
tags:
  - Array
  - Binary Search
  - Searching
---

## Java program to perform Binary Search

> Binary Search works for sorted arrays. Here, search-item is compared with the middle element of array. If the search-item matches with the element, search finishes. If search-item is less than middle, perform binary search in first-half of array, otherwise perform binary search in the latter half of the array.

```java
public class Main {
    public static void main (int n) {
        int[] a = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
        int flag = 0;
        int min = 0, max = a.length-1, mid = 0;
        
        while(min<=max) {
            mid = (min+max/2);
            if(n>a[mid]) {
                min = mid + 1;
            }
            else if (n<a[mid]) {
                max = mid - 1;
            }
            else {
                flag++;
                break;
            }
        }
        
        if(flag!=0){
            System.out.println("element found at : " + (mid+1));
        }
        else {
            System.out.println("element not found!");
        }
    }
}
```
