### Student Notes:

# Complexity Analysis in Programming

#### **Introduction to Complexity Analysis**

- **Complexity:** Refers to how an algorithm's resource usage (time or space) grows with the size of the input.
  - **Time Complexity:** How the runtime of an algorithm changes as the input size increases.
  - **Space Complexity:** How the memory usage of an algorithm changes as the input size increases.

#### **Types of Time Complexities**

1. **Constant Time \(O(1)\):**

   - **Definition:** The runtime is constant and does not depend on the input size.
   - **Example:** Accessing an element in an array.

   ```javascript
   function getElement(arr, index) {
     return arr[index]; // O(1)
   }
   ```

2. **Logarithmic Time \(O(\log n)\):**

   - **Definition:** The runtime grows logarithmically with the input size.
   - **Example:** Binary search in a sorted array.

   ```javascript
   function binarySearch(arr, target) {
     let left = 0;
     let right = arr.length - 1;
     while (left <= right) {
       let mid = Math.floor((left + right) / 2);
       if (arr[mid] === target) return mid;
       if (arr[mid] < target) left = mid + 1;
       else right = mid - 1;
     }
     return -1;
   }
   ```

3. **Linear Time \(O(n)\):**

   - **Definition:** The runtime grows linearly with the input size.
   - **Example:** Linear search through an unsorted array.

   ```javascript
   function linearSearch(arr, target) {
     for (let i = 0; i < arr.length; i++) {
       if (arr[i] === target) return i;
     }
     return -1;
   }
   ```

4. **Linearithmic Time \(O(n \log n)\):**

   - **Definition:** The runtime grows in proportion to \(n \log n\).
   - **Example:** Merge sort algorithm.

   ```javascript
   function mergeSort(arr) {
     if (arr.length <= 1) return arr;
     const mid = Math.floor(arr.length / 2);
     const left = mergeSort(arr.slice(0, mid));
     const right = mergeSort(arr.slice(mid));
     return merge(left, right);
   }

   function merge(left, right) {
     let result = [];
     let i = 0,
       j = 0;
     while (i < left.length && j < right.length) {
       if (left[i] < right[j]) result.push(left[i++]);
       else result.push(right[j++]);
     }
     return result.concat(left.slice(i)).concat(right.slice(j));
   }
   ```

5. **Quadratic Time \(O(n^2)\):**

   - **Definition:** The runtime grows quadratically with the input size.
   - **Example:** Bubble sort algorithm.

   ```javascript
   function bubbleSort(arr) {
     for (let i = 0; i < arr.length; i++) {
       for (let j = 0; j < arr.length - i - 1; j++) {
         if (arr[j] > arr[j + 1]) {
           [arr[j], arr[j + 1]] = [arr[j + 1], arr[j]];
         }
       }
     }
     return arr;
   }
   ```

6. **Cubic Time \(O(n^3)\):**

   - **Definition:** The runtime grows cubically with the input size.
   - **Example:** Algorithm with three nested loops.

   ```javascript
   function cubicExample(arr) {
     let n = arr.length;
     for (let i = 0; i < n; i++) {
       for (let j = 0; j < n; j++) {
         for (let k = 0; k < n; k++) {
           // Some operation
         }
       }
     }
   }
   ```

7. **Exponential Time \(O(2^n)\):**
   - **Definition:** The runtime grows exponentially with the input size.
   - **Example:** Recursive Fibonacci calculation.
   ```javascript
   function fibonacci(n) {
     if (n <= 1) return n;
     return fibonacci(n - 1) + fibonacci(n - 2);
   }
   ```

#### **Types of Space Complexities**

1. **Constant Space \(O(1)\):**

   - **Definition:** The space usage is constant and does not depend on the input size.
   - **Example:** Storing simple variables.

   ```javascript
   function constantSpaceExample() {
     let a = 5; // O(1)
   }
   ```

2. **Linear Space \(O(n)\):**

   - **Definition:** The space usage grows linearly with the input size.
   - **Example:** Storing elements in an array.

   ```javascript
   function linearSpaceExample(arr) {
     let result = [];
     for (let i = 0; i < arr.length; i++) {
       result.push(arr[i] * 2);
     }
     return result;
   }
   ```

3. **Space Complexity in Recursive Algorithms:**
   - **Definition:** Additional space is required for the function call stack.
   - **Example:** Recursive implementation of Fibonacci.
   ```javascript
   function recursiveExample(n) {
     if (n <= 1) return n;
     return recursiveExample(n - 1) + recursiveExample(n - 2);
   }
   // Recursive call stack adds to space complexity.
   ```

#### **Practical Scenarios**

- **Database Queries:** Efficient algorithms ensure faster data retrieval and manipulation.
- **Sorting Algorithms:** Choosing the right sorting algorithm based on data size can significantly affect performance.
- **Graph Algorithms:** Efficient pathfinding algorithms, like Dijkstra’s, are crucial for large networks and maps.

---
