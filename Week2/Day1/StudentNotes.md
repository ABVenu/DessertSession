### Student Notes:

# Basic Mathematics for Web Development

---

#### **1. Introduction to Basic Arithmetic**

**Objective**: Learn fundamental arithmetic operations and how to use them in JavaScript.

**Basic Arithmetic Operations**:

- **Addition**: `+` (e.g., `5 + 3 = 8`)
- **Subtraction**: `-` (e.g., `10 - 4 = 6`)
- **Multiplication**: `*` (e.g., `7 * 2 = 14`)
- **Division**: `/` (e.g., `20 / 4 = 5`)

**JavaScript Code Example**:

```javascript
// Addition
console.log(5 + 3); // 8

// Subtraction
console.log(10 - 4); // 6

// Multiplication
console.log(7 * 2); // 14

// Division
console.log(20 / 4); // 5
```

**Activity**: Create a simple calculator function that can perform addition, subtraction, multiplication, and division.

**Example Function**:

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

// Test the function
console.log(calculate(10, 5, "+")); // 15
console.log(calculate(10, 5, "-")); // 5
console.log(calculate(10, 5, "*")); // 50
console.log(calculate(10, 5, "/")); // 2
```

---

#### **2. Inbuilt Math Functions**

**Objective**: Learn about JavaScript’s `Math` object functions for rounding numbers and generating random numbers.

**Math Functions**:

- **`Math.floor()`**: Rounds down to the nearest integer.
  - Example: `Math.floor(4.7)` results in `4`.
- **`Math.ceil()`**: Rounds up to the nearest integer.
  - Example: `Math.ceil(4.2)` results in `5`.
- **`Math.round()`**: Rounds to the nearest integer.
  - Example: `Math.round(4.5)` results in `5`.
- **`Math.random()`**: Generates a random number between `0` (inclusive) and `1` (exclusive).
  - Example: `Math.random()` might give you `0.547`.

**Activity**: Write a function to generate a random integer between two values.

**Example Function**:

```javascript
function getRandomInt(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

// Test the function
console.log(getRandomInt(1, 10)); // Random integer between 1 and 10
```

---

#### **3. Ratios and Proportions**

**Objective**: Understand how to calculate and use ratios and proportions.

**Ratios**:

- A ratio compares two quantities. For example, the ratio of apples to oranges can be `3:2`.

**Proportions**:

- A proportion is an equation that states two ratios are equal. To solve a proportion, you can cross-multiply and divide.

**Example**:

- **Ratio**: If the ratio of apples to oranges is 3:2 and you have 9 apples, you have 6 oranges.
- **Proportion**: Solve for `x` in `4/5 = x/10`. To find `x`, use:

  ```javascript
  function solveProportion(a, b, c) {
    return (b * c) / a;
  }

  console.log(solveProportion(4, 5, 10)); // 12
  ```

---

#### **4. Percentages**

**Objective**: Learn how to calculate percentages and apply them to real-world scenarios.

**Percentage Calculation**:

- Find a percentage of a number by multiplying the number by the percentage (in decimal form).
  - Example: `20% of 150` is calculated as `150 * 0.20` which is `30`.

**Percentage Increase/Decrease**:

- To find the final amount after a percentage increase or discount:
  - **Increase**: `Original Amount + (Original Amount * Percentage)`
  - **Discount**: `Original Amount - (Original Amount * Percentage)`

**Example**:

- **Discount Calculation**: For a 15% discount on $200:

  ```javascript
  function calculatePercentage(amount, percentage) {
    return (amount * percentage) / 100;
  }

  function applyDiscount(price, discount) {
    return price - calculatePercentage(price, discount);
  }

  console.log(applyDiscount(200, 15)); // 170
  ```

---

#### **5. Exponents and Powers**

**Objective**: Learn to calculate powers and square roots using JavaScript.

**Exponents**:

- Use `Math.pow(base, exponent)` to calculate a number raised to a power.
  - Example: `Math.pow(2, 3)` results in `8`.

**Square Roots**:

- Use `Math.sqrt(number)` to find the square root of a number.
  - Example: `Math.sqrt(16)` results in `4`.

**Activity**: Write functions to calculate powers and square roots.

**Example Functions**:

```javascript
function power(base, exponent) {
  return Math.pow(base, exponent);
}

function squareRoot(number) {
  return Math.sqrt(number);
}

console.log(power(2, 3)); // 8
console.log(squareRoot(16)); // 4
```

---

**Why Mathematics is Important in Web Development**:

- **Layout Calculations**: Determine sizes and positions of elements.
- **Dynamic Content**: Calculate values for interactive content like games or data visualizations.
- **Data Analysis**: Process and analyze numerical data for reports and statistics.
- **Responsive Design**: Adjust layouts and styles based on screen size and resolution.

Mathematics helps in creating efficient, dynamic, and visually appealing web applications by enabling precise calculations and problem-solving.

---
