### Student Notes:

---

# Complexity Analysis in Programming

#### **1. Introduction to Complexity Analysis**

- **Complexity:** This refers to how an algorithm's resource usage (time or space) changes as the input size grows.
  - **Time Complexity:** Indicates how the execution time of an algorithm increases with input size.
  - **Space Complexity:** Indicates how the memory usage of an algorithm changes with input size.

#### **2. Need for Complexity Analysis**

- **Importance:** Analyzing complexity helps ensure that algorithms perform efficiently as data sizes grow. Inefficient algorithms can lead to slow performance and high resource usage.
- **Real-World Examples:**
  - **Twitter:** Slow performance with high user counts due to inefficient algorithms.
  - **MySpace:** Performance issues as the platform scaled up.
  - **Etsy:** Search functionality became slow under heavy load.

#### **3. Types of Time Complexities**

- **Constant Time \(O(1)\):**

  - **Definition:** The runtime is the same regardless of input size.
  - **Example:**

    ```javascript
    function getElement(arr, index) {
      return arr[index]; // O(1) operation
    }
    ```

- **Logarithmic Time \(O(\log n)\):**

  - **Definition:** Runtime increases logarithmically as input size grows.
  - **Example:**

    ```javascript
    function reduceArray(arr) {
      let result = 0;
      for (let i = arr.length; i > 0; i = Math.floor(i / 10)) {
        result += arr[i - 1];
      }
      return result;
    }
    ```

- **Linear Time \(O(n)\):**

  - **Definition:** Runtime increases linearly with input size.
  - **Example:**

    ```javascript
    function linearSearch(arr, target) {
      for (let i = 0; i < arr.length; i++) {
        if (arr[i] === target) return i;
      }
      return -1;
    }
    ```

- **Linearithmic Time \(O(n \log n)\):**

  - **Definition:** Runtime grows in proportion to \(n \log n\).
  - **Example:**

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

- **Quadratic Time \(O(n^2)\):**

  - **Definition:** Runtime grows quadratically with input size.
  - **Example:**

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

- **Cubic Time \(O(n^3)\):**

  - **Definition:** Runtime grows cubically with input size.
  - **Example:**

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

- **Exponential Time \(O(2^n)\):**

  - **Definition:** Runtime grows exponentially with input size.
  - **Examples:**

    - **Recursive Fibonacci:**

      ```javascript
      function fibonacci(n) {
        if (n <= 1) return n;
        return fibonacci(n - 1) + fibonacci(n - 2);
      }

      let count = 0;
      function fibonacci(n) {
        // console.log(`Calling fibonacci(${n})`); // Log the current call
        if (n <= 1) {
          count++;
          console.log(count);
          return n; // Base case: fibonacci(0) = 0, fibonacci(1) = 1
        }

        const result = fibonacci(n - 1) + fibonacci(n - 2); // Recursive case
        count++;
        console.log(count);
        return result;
      }

      // Testing the function
      console.log(`Result: fibonacci(5) = ${fibonacci(5)}`); // Outputs: 5
      ```

#### **4. Types of Space Complexities**

- **Constant Space \(O(1)\):**

  - **Definition:** Space usage does not depend on input size.
  - **Example:**

    ```javascript
    function constantSpaceExample(n) {
      let result = 0; // O(1) space usage
      for (let i = 0; i < n; i++) {
        result += i;
      }
      return result;
    }
    ```

- **Linear Space \(O(n)\):**

  - **Definition:** Space usage grows linearly with input size.
  - **Example:**

    ```javascript
    function linearSpaceExample(arr) {
      let result = [];
      for (let i = 0; i < arr.length; i++) {
        result.push(arr[i]); // O(n) space usage
      }
      return result;
    }
    ```

- **Space Complexity in Recursive Algorithms:**

  - **Definition:** Additional space for function call stack.
  - **Example:**

    ```javascript
    function recursiveFactorial(n) {
      if (n <= 1) return 1;
      return n * recursiveFactorial(n - 1); // O(n) stack space
    }
    ```

#### **5. Practical Scenarios and Optimal Complexity**

- **Database Queries:** Efficient algorithms ensure fast data retrieval. For example, use \(O(\log n)\) or \(O(n \log n)\) algorithms to handle large datasets efficiently.

- **Sorting and Searching:** For large datasets, use algorithms with lower time complexities like \(O(n \log n)\) (e.g., merge sort) rather than \(O(n^2)\) (e.g., bubble sort) to improve performance.

- **Pathfinding:** Use efficient algorithms like Dijkstra’s for large graphs to ensure quick pathfinding and avoid performance issues.

#### **6. Practical Exercises**

- **Implement Algorithms:** Practice writing and testing algorithms with different complexities to understand their performance.

- **Measure Performance:** Use `console.time` to measure how long different algorithms take to execute.

- **Analyze Space Complexity:** Observe and compare the memory usage of different algorithms to understand their space requirements.

---
