### **Questions on Time and Space Complexity**

#### **Easy Questions**

1. **Constant Time Complexity**
   - **Problem Statement:** Write a function that returns the first element of an array.
   - **Input:** `[5, 10, 15]`
   - **Output:** `5`

2. **Logarithmic Time Complexity**
   - **Problem Statement:** Implement a function that finds the position of a target value in a sorted array using binary search.
   - **Input 1:** `arr = [1, 2, 3, 4, 5]`, `target = 3`
   - **Output 1:** `2`
   - **Input 2:** `arr = [1, 3, 5, 7, 9]`, `target = 7`
   - **Output 2:** `3`

3. **Linear Time Complexity**
   - **Problem Statement:** Write a function that finds the maximum value in an array.
   - **Input:** `[4, 1, 7, 2, 9]`
   - **Output:** `9`

4. **Linear Time Complexity**
   - **Problem Statement:** Write a function that counts the number of even numbers in an array.
   - **Input:** `[1, 2, 3, 4, 5]`
   - **Output:** `2`

5. **Linearithmic Time Complexity**
   - **Problem Statement:** Implement merge sort to sort an array.
   - **Input:** `[3, 1, 4, 1, 5, 9]`
   - **Output:** `[1, 1, 3, 4, 5, 9]`

#### **Medium Questions**

6. **Quadratic Time Complexity**
   - **Problem Statement:** Write a function that finds all pairs of elements in an array whose sum is equal to a given value.
   - **Input 1:** `arr = [1, 2, 3, 4, 5]`, `target = 6`
   - **Output 1:** `[(1, 5), (2, 4)]`
   - **Input 2:** `arr = [0, -1, 2, -3, 1]`, `target = -2`
   - **Output 2:** `[(-3, 1), (-1, -1)]`

7. **Cubic Time Complexity**
   - **Problem Statement:** Write a function that performs a triply nested iteration over an array and prints each combination.
   - **Input:** `[1, 2, 3]`
   - **Output:** `[(1, 1, 1), (1, 1, 2), (1, 1, 3), ...]`

8. **Exponential Time Complexity**
   - **Problem Statement:** Implement a recursive function to compute the nth Fibonacci number.
   - **Input 1:** `n = 5`
   - **Output 1:** `5`
   - **Input 2:** `n = 6`
   - **Output 2:** `8`

9. **Space Complexity (Linear)**
   - **Problem Statement:** Write a function that duplicates every element in an array and returns the new array.
   - **Input:** `[1, 2, 3]`
   - **Output:** `[1, 1, 2, 2, 3, 3]`

10. **Space Complexity (Recursive)**
    - **Problem Statement:** Write a function that computes the factorial of a number recursively and shows the space complexity in terms of call stack depth.
    - **Input 1:** `n = 4`
    - **Output 1:** `24`
    - **Input 2:** `n = 5`
    - **Output 2:** `120`

---

These questions will help students understand and practice various types of time and space complexities by implementing different algorithms and analyzing their performance.


### **Complexity Analysis Questions**

#### **Question 1:**
**Problem Statement:** You are given an algorithm that performs a binary search on a sorted array to find a target value. The algorithm has a complexity of \(O(\log n)\). If you have an array of 1000 elements, how many steps will the algorithm take in the worst case?

- **A.** 10 steps
- **B.** 20 steps
- **C.** 1000 steps
- **D.** 500 steps

*Correct Answer:* A. 10 steps  
*Explanation:* Binary search divides the search space in half each time, so the number of steps is proportional to the logarithm of the number of elements.

#### **Question 2:**
**Problem Statement:** Consider the following function that uses a nested loop to process an array of size \(n\):

```javascript
function nestedLoop(arr) {
    for (let i = 0; i < arr.length; i++) {
        for (let j = 0; j < arr.length; j++) {
            // Some operation
        }
    }
}
```

What is the time complexity of this function?

- **A.** \(O(n)\)
- **B.** \(O(n^2)\)
- **C.** \(O(n \log n)\)
- **D.** \(O(2^n)\)

*Correct Answer:* B. \(O(n^2)\)  
*Explanation:* The function has two nested loops, each iterating over the array, leading to a quadratic time complexity.

#### **Question 3:**
**Problem Statement:** You have an algorithm that sorts an array using the Merge Sort algorithm. What is the time complexity of this sorting algorithm in the worst case?

- **A.** \(O(n)\)
- **B.** \(O(n \log n)\)
- **C.** \(O(n^2)\)
- **D.** \(O(2^n)\)

*Correct Answer:* B. \(O(n \log n)\)  
*Explanation:* Merge Sort is a divide-and-conquer algorithm that sorts the array by dividing it into smaller arrays, sorting them, and then merging them back together.

#### **Question 4:**
**Problem Statement:** Consider a function that recursively computes the factorial of a number:

```javascript
function factorial(n) {
    if (n <= 1) return 1;
    return n * factorial(n - 1);
}
```

What is the space complexity of this function?

- **A.** \(O(1)\)
- **B.** \(O(n)\)
- **C.** \(O(n^2)\)
- **D.** \(O(\log n)\)

*Correct Answer:* B. \(O(n)\)  
*Explanation:* The recursive function requires space proportional to the number of recursive calls on the call stack, which is linear with respect to \(n\).

#### **Question 5:**
**Problem Statement:** You are given an algorithm that uses a single loop to iterate over an array and performs a constant-time operation on each element. What is the time complexity of this algorithm?

- **A.** \(O(1)\)
- **B.** \(O(n)\)
- **C.** \(O(\log n)\)
- **D.** \(O(n^2)\)

*Correct Answer:* B. \(O(n)\)  
*Explanation:* The algorithm processes each element of the array once, leading to a linear time complexity.

---

These questions test students' ability to analyze and identify the time and space complexities of different algorithms.