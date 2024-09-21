# Complexity Analysis in Programming - II


#### **Question 1:**

**Problem Statement:** You are given an algorithm that performs a binary search on a sorted array to find a target value. The algorithm has a complexity of \(O(\log n)\). If you have an array of 1000 elements, how many steps will the algorithm take in the worst case?

- **A.** 10 steps
- **B.** 20 steps
- **C.** 1000 steps
- **D.** 500 steps

_Correct Answer:_ A. 10 steps  
_Explanation:_ Binary search divides the search space in half each time, so the number of steps is proportional to the logarithm of the number of elements.

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

_Correct Answer:_ B. \(O(n^2)\)  
_Explanation:_ The function has two nested loops, each iterating over the array, leading to a quadratic time complexity.

#### **Question 3:**

**Problem Statement:** You have an algorithm that sorts an array using the Merge Sort algorithm. What is the time complexity of this sorting algorithm in the worst case?

- **A.** \(O(n)\)
- **B.** \(O(n \log n)\)
- **C.** \(O(n^2)\)
- **D.** \(O(2^n)\)

_Correct Answer:_ B. \(O(n \log n)\)  
_Explanation:_ Merge Sort is a divide-and-conquer algorithm that sorts the array by dividing it into smaller arrays, sorting them, and then merging them back together.

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

_Correct Answer:_ B. \(O(n)\)  
_Explanation:_ The recursive function requires space proportional to the number of recursive calls on the call stack, which is linear with respect to \(n\).

#### **Question 5:**

**Problem Statement:** You are given an algorithm that uses a single loop to iterate over an array and performs a constant-time operation on each element. What is the time complexity of this algorithm?

- **A.** \(O(1)\)
- **B.** \(O(n)\)
- **C.** \(O(\log n)\)
- **D.** \(O(n^2)\)

_Correct Answer:_ B. \(O(n)\)  
_Explanation:_ The algorithm processes each element of the array once, leading to a linear time complexity.
---