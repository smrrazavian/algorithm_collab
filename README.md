# Algorithm Collab

AASAAM Algorithm &amp; Data Structures Collaboration notes and codes

## What is the goal of this collaboration?

The goal of this collaboration is to **learn** and **practice** algorithms and data structures **together**. We will be using **Python** and **JavaScript** as our main programming language.

## Why Algorithms and Data Structures?

Algorithms and data structures are the backbone of computer science and software development. Understanding these topics is crucial because they form the foundation for efficient problem-solving, enabling us to create better, faster, and more scalable software.

## Time Complexity

Time complexity is a measure of how the running time of an algorithm increases with the size of the input data.

1. **Big O Notation (O-notation):**
   - **Formal Definition:** The time complexity of an algorithm is said to be O(g(n)) if there exist positive constants C and n₀ such that for all values of n greater than or equal to n₀, the running time of the algorithm is at most C times the growth rate of the function g(n).
   - **Graphical Representation**: ![Big O Notation](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20200807150308/3363.png)
   - **Mathematical Definition:**

   ```plaintext
   f(n) is in O(g(n)) if there exist positive constants C and n₀ such that for all values of n ≥ n₀:
   0 ≤ f(n) ≤ C * g(n)

2. **Big Omega Notation (Ω-notation):**
   - **Formal Definition:** The time complexity of an algorithm is said to be Ω(g(n)) if there exist positive constants C and n₀ such that for all values of n greater than or equal to n₀, the running time of the algorithm is at least C times the growth rate of the function g(n).

   - **Graphical Representation**: ![Big Omega Notation](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20200807150659/3611.png)
   - **Mathematical Definition:**

   ```plaintext
   f(n) is in Ω(g(n)) if there exist positive constants C and n₀ such that for all values of n ≥ n₀:
   0 ≤ C * g(n) ≤ f(n)

3. **Big Theta Notation (Θ-notation):**
   - **Formal Definition:** The time complexity of an algorithm is said to be Θ(g(n)) if there exist positive constants C₁, C₂, and n₀ such that for all values of n greater than or equal to n₀, the running time of the algorithm is at least C₁ times the growth rate of the function g(n) and at most C₂ times the growth rate of the function g(n).
  
   - **Graphical Representation**: ![Big Theta Notation](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20200807150743/36955.png)

   - **Mathematical Definition:**

   ```plaintext
   f(n) is in Θ(g(n)) if there exist positive constants C₁, C₂, and n₀ such that for all values of n ≥ n₀:
   0 ≤ C₁ * g(n) ≤ f(n) ≤ C₂ * g(n)

### Some Common Time Complexities

| Notation | Name | Example |
| --- | --- | --- |
| O(1) | Constant | Accessing a specific element in an array by index |
| O(log n) | Logarithmic | Finding an element in a sorted array with a binary search |
| O(n) | Linear | Finding an element in an unsorted array with a linear search |
| O(n log n) | Log-linear | Sorting an array with merge sort or quick sort |
| O(n²) | Quadratic | Finding all possible pairs in an array with a nested loop |
| O(n³) | Cubic | Finding all possible triplets in an array with a triple nested loop |
| O(2ⁿ) | Exponential | Finding all subsets of a set with a power set algorithm |
| O(n!) | Factorial | Finding all permutations of a string or array with a permutation algorithm |
| O(nⁿ) | Polynomial | Finding all possible paths in a graph with a brute-force algorithm |

### Examples

1. **Constant Time Complexity (O(1)):**

   ```python
   def constant_time_complexity(arr):
       return arr[0]

2. **Linear Time Complexity (O(n)):**

   ```python
   def linear_time_complexity(arr):
       for i in arr:
           print(i)

3. **Quadratic Time Complexity (O(n²)):**

   ```python
   def quadratic_time_complexity(arr):
       for i in arr:
           for j in arr:
               print(i, j)

4. **Cubic Time Complexity (O(n³)):**

   ```python
   def cubic_time_complexity(arr):
       for i in arr:
           for j in arr:
               for k in arr:
                   print(i, j, k)

5. **Logarithmic Time Complexity (O(log n)):**

   ```python
   def logarithmic_time_complexity(arr):
       i = len(arr)
       while i > 0:
           print(arr[i])
           i = i // 2

6. **Log-Linear Time Complexity (O(n log n)):**

   ```python
   def log_linear_time_complexity(arr):
       for i in arr:
           j = len(arr)
           while j > 0:
               print(i, arr[j])
               j = j // 2

7. **Exponential Time Complexity (O(2ⁿ)):**

   ```python
   def exponential_time_complexity(n):
       if n <= 0:
           return 1
       return exponential_time_complexity(n - 1) + exponential_time_complexity(n - 1)

8. **Factorial Time Complexity (O(n!)):**

   ```python
   def factorial_time_complexity(n):
       if n <= 0:
           return 1
       return n * factorial_time_complexity(n - 1)

9. **Polynomial Time Complexity (O(nⁿ)):**

   ```python
   def polynomial_time_complexity(n):
       if n <= 0:
           return 1
       return n * polynomial_time_complexity(n)

### Exercises

These are some rough exercises that you use everyday in your codes. Try to find the time complexity of each one of them. some of them are really hard to find the exact time complexity, so you can just give a rough estimation.

1. :

   ```python
   def foo(n):
       i = 1
       while i < n:
           print(i)
           i = i * 2
   ```

   *Hint*: give attention to the while loop condition and the value of `i` in each iteration.

2. :

   ```python
   def foo(n):
       i = 1
       while i < n:
           j = 1
           while j < n:
               print(i, j)
               j = j * 3
           i = i * 2
   ```

   *Hint*: give attention to the while loop condition and the value of `i` and `j` in each iteration.
   Some people might think that the time complexity of this function is `O(n²)`, but it's not. It's actually `SOME THING THAT YOU ARE GONNA FIND OUT`.

## Space Complexity

## Data Structures

### Array

### Linked List

### Stack

### Queue

### Hash Table

### Tree

### Heap

## Algorithms

### Sorting

### Searching

### Graph

### Greedy

### Dynamic Programming

### Recursion

### Divide and Conquer

### Backtracking

### BFS

### DFS
