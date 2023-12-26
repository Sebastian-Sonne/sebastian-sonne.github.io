---
layout:     post
title:      "[Java] Fibonacci Sequence"
subtitle:   " \"A simple java class to print n Fibonacci numvers\""
date:       2023-12-25 12:00:00
author:     "Sebastian Sonne"
header-img: "img/in-post/fibonacci.jpeg"
catalog: true
tags:
    - java
    - fibonacci
    - code
---
The **`Fibonacci sequence`** is a series of numbers in which each number (known as a Fibonacci number) is the sum of the two preceding ones.
It typically starts with 0 and 1. The sequence goes: `0, 1, 1, 2, 3, 5, 8, 13, 21`, and so on.

<hr>

Mathematically, it is defined by the recurrence relation:

#### `F(n) = F(n-1) + F(n-2)`

where `F(n)` is the nth Fibonacci number, `F(0) = 0`, and `F(1) = 1`.

Here's a breakdown of how the sequence is formed:

1. **Initialization**: The sequence starts with 0 and 1.

    ```java
    F(0) = 0
    F(1) = 1
    ```

2. **Iteration**: Each subsequent number in the sequence is the sum of the two preceding ones.

    ```java
    F(2) = F(1) + F(0) = 1 + 0 = 1
    F(3) = F(2) + F(1) = 1 + 1 = 2
    F(4) = F(3) + F(2) = 2 + 1 = 3
    //And so on...
    ```

<hr>

The Fibonacci sequence has fascinating properties and appears in various `natural phenomena`, including the `arrangement of leaves` on a stem, the `spiral pattern` of pinecones, the `layout of sunflower seeds`, and even in the `proportions of the human body`. It's also prevalent in art, architecture, and music.

Enough with the preamble, let's write some Java code! Below, you'll find a snippet that brings the `Fibonacci sequence` to life. No frills, just the nuts and bolts of making numbers dance to a Fibonacci beat.

```java
public class Fibonacci {

    public static void main(String[] args) {
        // Example: Generate Fibonacci sequence up to the 10th term
        int n = 10;
        int[] result = generateFibonacci(n);
        printArray(result);
    }

    public static int[] generateFibonacci(int n) {
        // Generate Fibonacci sequence up to the nth term
        int[] fibSequence = new int[n];
        fibSequence[0] = 0;
        fibSequence[1] = 1;
        for (int i = 2; i < n; i++) {
            fibSequence[i] = fibSequence[i - 1] + fibSequence[i - 2];
        }
        return fibSequence;
    }

    public static void printArray(int[] arr) {
        // Print the elements of an array
        System.out.print("[");
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i]);
            if (i < arr.length - 1) {
                System.out.print(", ");
            }
        }
        System.out.println("]");
    }
}
```

This Java code defines a `Fibonacci` class with a `main` method that demonstrates how to generate and print the Fibonacci sequence up to the 10th term. The `generateFibonacci` method calculates the sequence, and the `printArray` method is used to print the elements of an array.
When run, this is the output:

> [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]

Feel free to use and modify this code as needed!