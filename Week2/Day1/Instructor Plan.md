### Lecture Name:

# Basic Mathematics for Web Development

### Part A Session Flow Breakdown

**Objective**: Understand and implement fundamental mathematical operations and concepts using JavaScript, and learn how these concepts are applied in web development.

---

#### **Session Flow**:

1. **Introduction to Basic Arithmetic**

   - **Concepts Covered**: Addition, subtraction, multiplication, and division.
   - **JavaScript Functions**: `+`, `-`, `*`, `/`.
   - **Example**: Simple calculator for basic operations.
   - **Activity**: Demonstrate basic arithmetic operations using JavaScript and ask students to solve basic problems.

2. **Inbuilt Math Functions**

   - **Concepts Covered**: `Math.floor()`, `Math.ceil()`, `Math.round()`, `Math.random()`.
   - **JavaScript Functions**:
     - `Math.floor()`: Rounds down to the nearest integer.
     - `Math.ceil()`: Rounds up to the nearest integer.
     - `Math.round()`: Rounds to the nearest integer.
     - `Math.random()`: Generates a random number between 0 and 1.
   - **Example**: Rounding decimal values and generating random numbers.
   - **Activity**: Create functions to generate random integers within a specified range and round numbers.

3. **Ratios and Proportions**

   - **Concepts Covered**: Calculating ratios and proportions.
   - **JavaScript Functions**: Arithmetic operations and basic functions for ratio calculations.
   - **Example**: Calculate the ratio of two numbers and solve proportion problems.
   - **Activity**: Write a function to determine the ratio between two values and solve a proportional problem.

4. **Percentages**

   - **Concepts Covered**: Calculating percentages, percentage increase/decrease.
   - **JavaScript Functions**: Arithmetic operations for percentage calculations.
   - **Example**: Calculate 20% of a number and determine the final price after a 15% discount.
   - **Activity**: Implement a function to calculate percentage increase and decrease.

5. **Exponents and Powers**

   - **Concepts Covered**: Using exponents and powers, square roots.
   - **JavaScript Functions**: `Math.pow()`, `Math.sqrt()`.
   - **Example**: Calculate the power of a number and find the square root.
   - **Activity**: Create a function to compute powers and square roots.

6. **Practical Applications in Web Development**
   - **Concepts Covered**: Applying mathematical calculations to web design and development.
   - **Examples**:
     - Calculating layout dimensions.
     - Adjusting element sizes based on percentages.
   - **Activity**: Use JavaScript to solve real-world problems such as resizing elements based on user input or calculating the layout dimensions.

---

#### **Hands-On Exercise**:

1.  **Basic Calculator**: Create a simple calculator that performs addition, subtraction, multiplication, and division.
2.  **Random Number Generator**: Write a function that generates a random number between two specified values.
3.  **Percentage Calculator**: Implement a function to calculate percentages and apply it to a price for discount calculations.
4.  **Power and Root Calculator**: Develop functions to calculate the power of a number and its square root.

---

### Part B Instructor Session Content/Notes

---

#### **1. Introduction to Basic Arithmetic**

**Objective**: Introduce fundamental arithmetic operations and their implementation in JavaScript.

**Concepts Covered**:

- **Addition**: `+`
- **Subtraction**: `-`
- **Multiplication**: `*`
- **Division**: `/`

**JavaScript Functions**:

- Basic arithmetic operators are used directly in JavaScript to perform calculations.

**Examples**:

1. **Addition**: `5 + 3` results in `8`.
2. **Subtraction**: `10 - 4` results in `6`.
3. **Multiplication**: `7 * 2` results in `14`.
4. **Division**: `20 / 4` results in `5`.

**Activity**:

- **Create a Simple Calculator**:
  - Write a JavaScript function that takes two numbers and an operator as inputs and returns the result of the operation.
  - Example function:
    ```javascript
    function calculate(num1, num2, operator) {
      switch (operator) {
        case "+":
          return num1 + num2;
        case "-":
          return num1 - num2;
        case "*":
          return num1 * num2;
        case "/":
          return num1 / num2;
        default:
          return "Invalid operator";
      }
    }
    ```
  - Test with various operations and inputs.

---

#### **2. Inbuilt Math Functions**

**Objective**: Demonstrate the use of JavaScript’s `Math` object functions for rounding and random number generation.

**Concepts Covered**:

- **`Math.floor()`**: Rounds down to the nearest integer.
- **`Math.ceil()`**: Rounds up to the nearest integer.
- **`Math.round()`**: Rounds to the nearest integer.
- **`Math.random()`**: Generates a random floating-point number between `0` (inclusive) and `1` (exclusive).

**Examples**:

1. **`Math.floor()`**: `Math.floor(4.7)` results in `4`.
2. **`Math.ceil()`**: `Math.ceil(4.2)` results in `5`.
3. **`Math.round()`**: `Math.round(4.5)` results in `5`.
4. **`Math.random()`**: Generates a random number, e.g., `0.547`.

**Activity**:

- **Generate Random Integers**:
  - Write a function to generate a random integer between two specified values:
    ```javascript
    function getRandomInt(min, max) {
      return Math.floor(Math.random() * (max - min + 1)) + min;
    }
    ```
  - Test the function with different ranges.

---

#### **3. Ratios and Proportions**

**Objective**: Explain how to calculate and use ratios and proportions in JavaScript.

**Concepts Covered**:

- **Ratios**: Comparison between two quantities.
- **Proportions**: Solving problems where two ratios are set equal.

**Examples**:

1. **Ratio**: If the ratio of apples to oranges is 3:2, and you have 9 apples, you have 6 oranges.
2. **Proportion**: Solve for x in the proportion `4/5 = x/10`.

**Activity**:

- **Calculate Ratios and Proportions**:

  - Write a function to calculate the ratio and solve for a missing value in a proportion:

    ```javascript
    function calculateRatio(a, b) {
      return a / b;
    }

    function solveProportion(a, b, c) {
      return (b * c) / a;
    }
    ```

  - Test with different ratios and proportions.

---

#### **4. Percentages**

**Objective**: Understand how to calculate percentages, including increases and decreases.

**Concepts Covered**:

- **Percentage Calculation**: Finding a percentage of a number.
- **Percentage Increase/Decrease**: Calculating how much a value has increased or decreased in percentage terms.

**Examples**:

1. **Calculate 20% of 150**: `150 * 0.20` results in `30`.
2. **Calculate a 15% discount on $200**: `200 * 0.15` results in `30`. Final price: `200 - 30` = `170`.

**Activity**:

- **Percentage Calculator**:

  - Write a function to calculate the percentage of a number and apply it to a price:

    ```javascript
    function calculatePercentage(amount, percentage) {
      return (amount * percentage) / 100;
    }

    function applyDiscount(price, discount) {
      return price - calculatePercentage(price, discount);
    }
    ```

  - Test with various amounts and discount rates.

---

#### **5. Exponents and Powers**

**Objective**: Use JavaScript to calculate powers and square roots.

**Concepts Covered**:

- **Exponentiation**: Raising a number to a power.
- **Square Roots**: Finding the square root of a number.

**Examples**:

1. **Exponentiation**: `Math.pow(2, 3)` results in `8`.
2. **Square Root**: `Math.sqrt(16)` results in `4`.

**Activity**:

- **Power and Root Calculator**:

  - Write functions to calculate powers and square roots:

    ```javascript
    function power(base, exponent) {
      return Math.pow(base, exponent);
    }

    function squareRoot(number) {
      return Math.sqrt(number);
    }
    ```

  - Test with different base and exponent values, and find square roots of various numbers.

---

**Instructor Tips**:

- **Engage with Examples**: Use relatable examples to illustrate each concept.
- **Encourage Experimentation**: Allow students to modify examples and test different values.
- **Highlight Real-World Use**: Emphasize how these mathematical operations are used in web development tasks.

This detailed plan provides a structured approach to teaching fundamental mathematics and its application using JavaScript, ensuring students gain practical and theoretical knowledge.
