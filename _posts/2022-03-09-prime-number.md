---
published: true
categories:
    - Numbers
tags:
    - Maths
    - Numerical
---
## Java Program to check whether a given number is prime or not

```java
public class Main {
    /*
     * A Number is a prime number if it is divisible only by itself and 1
     */
    public static void main(String[] args) {
        int number = 26; // Can be any Integer
        int count = 0;
        for (int i = 1; i <= number; i++) {
            if (number % i == 0) {
                count++;
            }
        }
        if (count == 2) {
            System.out.println("Prime Number");
        } else {
            System.out.println("Not a Prime Number");
        }
    }
}
```
