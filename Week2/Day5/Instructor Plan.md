### Lecture Name:

# Problem-Solving Strategies

### Part A Session Flow Breakdown

---

#### **1. Introduction to Problem-Solving (10 mins)**

- **Instructional Strategy**:

  - Start by explaining how breaking problems into smaller steps is a common approach to everyday tasks (e.g., cooking, planning an event).
  - Relate this to programming, where a large task can be daunting, but smaller, well-defined sub-tasks are easier to handle.

- **Prompts**:
  - Ask students to think of a large problem they faced and how they tackled it step by step.

---

#### **2. Steps for Solving a Problem (15 mins)**

- **Instructional Strategy**:

  - Provide a structured way to approach coding problems: Understanding -> Planning -> Executing.
  - Use simple problems to illustrate these steps, such as "find the largest number in an array."

- **Activity**:
  - As a group, take a simple problem and go through these steps together, asking students for input at each stage.
  - Draw a flowchart to visually explain how the logic flows.

---

#### **3. Decision Making in Programming (20 mins)**

- **Instructional Strategy**:

  - Explain how conditional statements (`if`, `else`, `else if`) allow decisions in code.
  - Walk through a few examples with increasing complexity.

- **Prompts**:
  - Ask students why decisions are important in real-world programming, such as deciding between different routes or actions based on user input.
- **Code Discussion**:
  - Present each snippet and ask questions to check for understanding.
  - For the `canVote` example, ask students to provide different inputs and predict the output.

---

#### **4. Breaking Down Algorithms (25 mins)**

- **Instructional Strategy**:
  - Explain that even complex algorithms can be broken down into smaller steps.
  - Present a problem, write the pseudo-code together, and then implement the solution.
- **Activity**:
  - Go through each example (Linear Search, Count Occurrences, Reverse Array) one by one.
  - After each solution is presented, ask students to explain how they would break it down in their own words.
  - Test the solution with various inputs to see if students understand how it works.

---

#### **5. Group Activity (15-20 mins)**

- **Instructional Strategy**:

  - Assign groups a simple problem that they have to break down, write pseudo-code for, and then implement.
  - Guide groups if they get stuck, but encourage them to think about the problem first before jumping into the code.

- **Prompts**:
  - After they complete the activity, ask groups to explain their pseudo-code and how they broke down the problem.
  - If time permits, ask them to explain how they approached solving the problem differently from other groups.

---

#### **6. Conclusion and Homework (5-10 mins)**

- **Instructional Strategy**:

  - Recap the key points about problem-solving strategies: breaking problems down, decision-making, and executing a plan in code.
  - Provide clear instructions for homework.

- **Prompts**:
  - Ask students to summarize what they’ve learned in the session.
  - Give them hints or examples related to the palindrome problem to help with their homework.

---

---

### Part B Instructor Session Content/Notes

1. **Introduction to Problem-Solving**

   - Explain the importance of problem-solving in programming.
   - Introduce the concept of breaking complex problems into smaller tasks.

2. **Steps for Solving a Problem**

   - Walk students through the three key steps:
     1. **Understanding the Problem**: Identify inputs and expected outputs.
     2. **Plan**: Use pseudo-code or flowcharts to plan the solution.
     3. **Execute**: Convert the plan into code and test.
   - **Introduce the concept of a Dry Run**:
     - Explain how dry running involves walking through the pseudo-code or logic manually, using sample inputs to ensure it works as expected.

3. **Decision Making in Code**

   - Introduce basic conditional statements using `if`, `else if`, and `else`.
   - Discuss the use of logical operators for complex decision-making.

4. **Example 1: Check if a Number is Positive, Negative, or Zero**

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

5. **Example 2: Linear Search**

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

6. **Decision-Making Examples (Nested Conditions & Logical Operators)**

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

7. **Intercartion Activity**

   - Provide a good problem statement, tell students to write the psudo code in their books, then after sometime, with the help of the students and solve it by the following steps.
     1. Write down all the steps.
     2. Plan using pseudo-code (in comments).
     3. Code the solution.
     4. **Dry Run** their solution before testing it.

8. **Wrap-Up and Homework Assignment**
   - Review key concepts of breaking problems into smaller parts, using pseudo-code, dry running code, and implementing decisions.
   - Homework: Write a function to check if a word is a palindrome, with full steps, pseudo-code, and dry-run the solution.

---
