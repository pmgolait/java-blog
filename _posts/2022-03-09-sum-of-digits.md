---
published: true
categories:
    - Numbers
tags:
    - Maths
    - Numerical
---
## Java Program to find sum of given digits

```java
public class Main { 
    public static void main(String[] args) {
        int n = 1921; // Can be any number
        int sum = 0;

        while (n != 0) {
            sum = sum + n % 10;
            n = n / 10;
        }
        System.out.println("Sum of Digits is : " + sum);
    }
}
```
