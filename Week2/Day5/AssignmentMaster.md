### **Instructor Notes: Problem-Solving Strategies**

---

#### **Session Overview:**

**Objective**: To teach students how to break down problems into smaller, manageable parts using problem-solving strategies and implement them in code. This session will focus on understanding problems, creating a plan (pseudo-code or flowchart), and executing the plan in code. The session will also introduce the concept of **Dry Run** for debugging and testing.

---

### **Session Flow:**

1. **Introduction to Problem-Solving** (5 minutes)

   - Explain the importance of problem-solving in programming.
   - Introduce the concept of breaking complex problems into smaller tasks.

2. **Steps for Solving a Problem** (10 minutes)

   - Walk students through the three key steps:
     1. **Understanding the Problem**: Identify inputs and expected outputs.
     2. **Plan**: Use pseudo-code or flowcharts to plan the solution.
     3. **Execute**: Convert the plan into code and test.
   - **Introduce the concept of a Dry Run**:
     - Explain how dry running involves walking through the pseudo-code or logic manually, using sample inputs to ensure it works as expected.

3. **Decision Making in Code** (10 minutes)

   - Introduce basic conditional statements using `if`, `else if`, and `else`.
   - Discuss the use of logical operators for complex decision-making.

4. **Example 1: Check if a Number is Positive, Negative, or Zero** (15 minutes)

   - Walk through problem-solving steps:
     1. **Understanding the problem**: We need to check the sign of a number.
     2. **Plan**: Use `if-else` to compare the number with zero.
     3. **Pseudo-code**: Write the steps in comments before the code.
     4. **Dry Run**: Perform a dry run of the pseudo-code with sample inputs (e.g., positive number, negative number, zero) to show how it behaves before actual execution.
   - Code Example:

     ```javascript
     // Step 1: Understand the problem
     // We need to check if a number is positive, negative, or zero.

     // Step 2: Plan
     // If number > 0, print "positive".
     // If number < 0, print "negative".
     // Otherwise, print "zero".

     function checkNumber(num) {
       // Step 3: Execute
       if (num > 0) {
         console.log("The number is positive.");
       } else if (num < 0) {
         console.log("The number is negative.");
       } else {
         console.log("The number is zero.");
       }
     }

     // Dry Run Example
     // Input: 5 => Output: "The number is positive."
     // Input: -3 => Output: "The number is negative."
     // Input: 0 => Output: "The number is zero."
     ```

5. **Example 2: Linear Search** (15 minutes)

   - Walk through steps:
     1. **Understanding the problem**: Find a target number in an array.
     2. **Plan**: Loop through the array and compare each element to the target.
     3. **Pseudo-code**: Outline the steps in comments.
     4. **Dry Run**: Use sample arrays and targets to simulate the algorithm's behavior step by step.
   - Code Example:

     ```javascript
     // Step 1: Understand the problem
     // Find the index of a target number in the array.

     // Step 2: Plan
     // Loop through the array.
     // If an element equals the target, return the index.
     // If no match is found, return -1.

     function linearSearch(arr, target) {
       // Step 3: Execute
       for (let i = 0; i < arr.length; i++) {
         if (arr[i] === target) {
           return i; // Target found, return index
         }
       }
       return -1; // Target not found
     }

     // Dry Run Example
     // Input: [10, 20, 30], target = 20
     // Step 1: Check arr[0] = 10 => Not match
     // Step 2: Check arr[1] = 20 => Match, return index 1
     ```

6. **Decision-Making Examples (Nested Conditions & Logical Operators)** (15 minutes)

   - Discuss how decision-making can be used in real-world problems (e.g., assigning grades, checking voting eligibility).
   - **Example**: Assign grades based on scores.

     ```javascript
     // Step 1: Understand the problem
     // Based on a score, assign a grade (A, B, C, D).

     // Step 2: Plan
     // If score >= 90, grade = A.
     // If score >= 80, grade = B.
     // If score >= 70, grade = C.
     // Else, grade = D.

     function assignGrade(score) {
       // Step 3: Execute
       if (score >= 90) {
         console.log("Grade: A");
       } else if (score >= 80) {
         console.log("Grade: B");
       } else if (score >= 70) {
         console.log("Grade: C");
       } else {
         console.log("Grade: D");
       }
     }

     // Dry Run Example
     // Input: 85 => Output: "Grade: B"
     // Input: 92 => Output: "Grade: A"
     ```

7. **Group Activity** (20 minutes)

   - Students will be tasked to write pseudo-code and implement a function that checks if a number exists in an array. They will work in groups to:
     1. Write down all the steps.
     2. Plan using pseudo-code (in comments).
     3. Code the solution.
     4. **Dry Run** their solution before testing it.

8. **Wrap-Up and Homework Assignment** (5 minutes)
   - Review key concepts of breaking problems into smaller parts, using pseudo-code, dry running code, and implementing decisions.
   - Homework: Write a function to check if a word is a palindrome, with full steps, pseudo-code, and dry-run the solution.

---

### **Student Notes: Problem-Solving Strategies**

---

### **1. Introduction to Problem-Solving**

In programming, problem-solving involves breaking down large problems into smaller, manageable tasks. This allows you to focus on solving one part at a time before piecing everything together.

---

### **2. Steps for Solving a Problem**

To solve any problem, follow these three steps:

1. **Understanding the Problem**:

   - Identify the inputs and expected outputs.

   **Example**: If the problem asks to find a number in an array, the inputs are the array and the target number, and the output is the index of the number (or -1 if it’s not found).

2. **Plan**:

   - Write **pseudo-code**: Describe the steps in plain language, focusing on the logic rather than the syntax.
   - Optionally, use flowcharts to visualize how different parts of the program will work.
   - **Dry Run**: Before implementing the solution, manually walk through the pseudo-code with sample inputs to predict the outcome.

3. **Execute**:
   - Turn the pseudo-code into actual code, and test it to ensure it works correctly.

---

### **3. Example: Check if a Number is Positive, Negative, or Zero**

- **Step 1: Understand the problem**: We need to determine if a number is positive, negative, or zero.
- **Step 2: Plan**:
  - If the number is greater than 0, it’s positive.
  - If it’s less than 0, it’s negative.
  - If it’s equal to 0, it’s zero.
- **Step 3: Dry Run**: Manually test the pseudo-code with different values to ensure the logic is correct.
- **Step 4: Execute**: Write the code based on the plan.

**Code**:

```javascript
// Step 1: Understand the problem
// We need to check if a number is positive, negative, or zero.

// Step 2: Plan
// If number > 0, print "positive".
// If number < 0, print "negative".
// Otherwise, print "zero".

function checkNumber(num) {
  // Step 4: Execute
  if (num > 0) {
    console.log("The number is positive.");
  } else if (num < 0) {
    console.log("The number is negative.");
  } else {
    console.log("The number is zero.");
  }
}

// Dry Run Example
// Input: 5 => Output: "The number is positive."
// Input: -3 => Output: "The number is negative."
// Input: 0 => Output: "The number is zero."
```

---

### **4. Decision Making in Code**

In programming, decision-making allows the program to choose between different actions based on conditions. We use conditional statements like `if-else` to implement this.

**Example: Assign Grades Based on Scores**

- **Step 1: Understand the problem**: Given a score, assign a grade.
- **Step 2: Plan**:
  - If the score is 90 or above, assign grade A.
  - If it’s 80 or above, assign grade B.
  - If it’s 70 or above, assign grade C.
  - Otherwise, assign grade D.
- **Step 3: Dry Run**:
  Go through the logic with different scores to see what grades would be assigned.
- **Step 4: Execute**: Implement the logic in code.

**Code**:

```javascript
function assignGrade(score) {
  // Step 3: Execute
  if (score >= 90) {
    console.log("Grade: A");
  } else if (score >= 80) {
    console.log("Grade: B");
  } else if (score >= 70) {
    console.log("Grade: C");
  } else {
    console.log("Grade: D");
  }
}

// Dry Run Example
// Input: 85 => Output: "Grade: B"
// Input: 92 => Output: "Grade: A"
```

---

### **5. Group Activity**

Work in groups to implement a function that checks if a number exists in an array. Follow these steps:

1. Write down the steps in pseudo-code.
2. Plan out the logic.
3. Write the code.
4. Perform a **Dry Run** with sample inputs to ensure it works correctly before testing it.

---

### **6. Homework Assignment**

Write a function to check if a word is a palindrome (reads the same forward and backward). Make sure to:

- Outline all steps.
- Write pseudo-code.
- Perform a dry run of your solution.

---

By understanding these strategies, you will be better equipped to tackle programming challenges effectively!
