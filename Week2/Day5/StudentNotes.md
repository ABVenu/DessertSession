### Student Notes:

---

# Problem-Solving Strategies

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
