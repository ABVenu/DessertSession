### Lecture Name:

# Logical Reasoning using JavaScript

### Part A Session Flow Breakdown

**Objective:**  
The session focuses on using logical reasoning to solve practical problems in JavaScript. Students will apply logical concepts like encoding/decoding, data sufficiency, clocks/calendars, Boolean algebra, directions, and cipher/decipher strings, using basic JavaScript principles such as loops, conditionals, and the `Date` object.

---

### **Session Breakdown**

1. **Introduction to Logical Reasoning in JavaScript**

   - **Overview**: Discuss the role of logical reasoning in programming and how it applies to JavaScript problem-solving.
   - **Example**: Use a simple route-planning example to demonstrate decision-making with JavaScript’s `if-else` and loops.

2. **Encoding and Decoding**

   - **Explanation**: Introduce encoding/decoding and explain their use in web applications (e.g., Base64 encoding, URL encoding).
   - **Example**: Demonstrate Base64 encoding and decoding in JavaScript.
   - **Exercise**: Students create functions to encode/decode strings for secure data transmission or URL handling.

3. **Cipher and Decipher Strings**

   - **Explanation**: Introduce ciphers as a method for securing data (e.g., Caesar cipher for encryption).
   - **Example**: Walk through creating a Caesar cipher in JavaScript to encode and decode text by shifting characters.
   - **Exercise**: Implement cipher and decipher functions, shifting characters by a given number of positions in the alphabet.

4. **Data Sufficiency**

   - **Explanation**: Explore how to determine whether enough data is available to solve a problem (e.g., form validation).
   - **Example**: Write a function that checks whether enough input is provided to calculate the area of a rectangle.
   - **Exercise**: Create sufficiency checks for various problems like calculating perimeters or tax rates based on input data.

5. **Clocks and Calendars (with Date Function)**

   - **Explanation**: Use the JavaScript `Date` object to handle date and time-related tasks.
   - **Example**: Calculate the number of days between two dates, or find out what day of the week a certain date falls on.
   - **Exercise**: Students calculate the difference between two dates, find deadlines, or convert between time zones using the `Date` object.

6. **Boolean Algebra**

   - **Explanation**: Discuss Boolean operations and how they’re applied in real-world problems such as form validation and access control.
   - **Example**: Use Boolean logic to check multiple conditions, such as whether a user’s input satisfies all criteria for a valid password.
   - **Exercise**: Students practice combining conditions to validate data using Boolean operators.

7. **Directions**

   - **Explanation**: Calculate positions based on directional movements (North, South, East, West).
   - **Example**: Write a JavaScript function to track a person’s movements and calculate the final position.
   - **Exercise**: Students build a function to simulate navigation based on a series of directional moves.

8. **Practical Application Review**

   - Review the practical use of encoding/decoding, cipher/decipher, Boolean logic, date/time management, and directional logic in real-world applications like web apps and games.

9. **Q&A and Wrap-Up**
   - Open discussion for questions and clarify concepts.
   - Assign a brief exercise for homework to reinforce the session’s concepts.

---

### Part B Instructor Session Content/Notes

---

#### **1. Introduction to Logical Reasoning in JavaScript**

- **Instructor Explanation**:

  - Logical reasoning helps solve real-world problems through structured thinking and can be directly translated into code using JavaScript.
  - Explain how logical structures like conditionals and loops are used to apply logic in code.

- **Example**:  
  Use `if-else` conditions to simulate decision-making (e.g., a user selecting between transportation options).

  ```javascript
  function chooseTransport(option) {
    if (option === "walk") {
      return "You chose to walk.";
    } else if (option === "drive") {
      return "You chose to drive.";
    } else {
      return "Please choose a valid option.";
    }
  }
  console.log(chooseTransport("walk")); // Output: "You chose to walk."
  ```

#### **2. Encoding and Decoding**

- **Practical Use Cases**:

  - Base64 encoding is used to safely transmit data, especially in authentication or web APIs.
  - URL encoding ensures that data can be safely included in URLs.

- **JavaScript Example**:

  ```javascript
  let encoded = btoa("Hello World!"); // Base64 encode
  let decoded = atob(encoded); // Base64 decode
  console.log(encoded); // Output: "SGVsbG8gV29ybGQh"
  console.log(decoded); // Output: "Hello World!"
  ```

- **Exercise**:  
  Students will write functions that encode and decode user inputs (e.g., URL-encoded strings).

#### **3. Cipher and Decipher Strings**

- **Explanation**:

  - A cipher is a method for transforming data into an unreadable format to secure it (encryption).
  - The Caesar cipher shifts letters in the alphabet by a certain number to encode or decode text.

- **JavaScript Example (Caesar Cipher)**:

  **Cipher**:

  ```javascript
  function cipher(str, shift) {
    let result = "";
    for (let i = 0; i < str.length; i++) {
      let charCode = str.charCodeAt(i);
      if (charCode >= 65 && charCode <= 90) {
        // Uppercase letters
        result += String.fromCharCode(((charCode - 65 + shift) % 26) + 65);
      } else if (charCode >= 97 && charCode <= 122) {
        // Lowercase letters
        result += String.fromCharCode(((charCode - 97 + shift) % 26) + 97);
      } else {
        result += str[i]; // Non-alphabet characters remain the same
      }
    }
    return result;
  }
  console.log(cipher("hello", 3)); // Output: "khoor"
  ```

  **Decipher**:

  ```javascript
  function decipher(str, shift) {
    return cipher(str, 26 - shift); // Reverse the cipher shift
  }
  console.log(decipher("khoor", 3)); // Output: "hello"
  ```

- **Exercise**:  
  Implement cipher and decipher functions to encode/decode messages using different shift values.

#### **4. Data Sufficiency**

- **Practical Use Case**:

  - Determine whether all required data is present before solving a problem (e.g., form validation).

- **JavaScript Example**:

  ```javascript
  function calculateArea(length, width) {
    if (!length || !width) {
      return "Insufficient data to calculate area.";
    }
    return length * width;
  }
  console.log(calculateArea(5, 3)); // Output: 15
  console.log(calculateArea(5)); // Output: "Insufficient data to calculate area."
  ```

- **Exercise**:  
  Write functions that check whether sufficient data is provided to solve problems like calculating volumes or prices.

#### **5. Clocks and Calendars (Date Function)**

- **Practical Use Case**:

  - Scheduling events, calculating deadlines, and working with date/time in applications.

- **JavaScript Example**:

  ```javascript
  function daysBetween(date1, date2) {
    let diffInTime = new Date(date2) - new Date(date1);
    let diffInDays = diffInTime / (1000 * 3600 * 24);
    return Math.abs(diffInDays);
  }
  console.log(daysBetween("2024-09-18", "2024-09-25")); // Output: 7
  ```

- **Exercise**:  
  Students will write functions that calculate time differences between two dates or convert time between zones using the `Date` object.

#### **6. Boolean Algebra**

- **Practical Use Case**:

  - Boolean logic is important for validating input data and controlling access based on multiple conditions.

- **JavaScript Example**:

  ```javascript
  function isEligible(age, hasLicense) {
    return age >= 18 && hasLicense;
  }
  console.log(isEligible(19, true)); // Output: true
  console.log(isEligible(17, true)); // Output: false
  ```

- **Exercise**:  
  Create functions that combine multiple conditions (e.g., check whether a user meets multiple criteria).

#### **7. Directions**

- **Practical Use Case**:

  - Navigation systems or tracking systems often involve calculating a final position based on directional movements.

- **JavaScript Example**:
  ```javascript
  function finalPosition(movements) {
    let x = 0,
      y = 0;
    for (let i = 0; i < movements.length; i++) {
      let move = movements[i];
      if (move === "N") {
        y++;
      } else if (move === "S") {
        y--;
      } else if (move === "E") {
        x++;
      } else if (move === "W") {
        x--;
      }
    }
    return { x, y };
  }
  console.log(finalPosition(["N", "E", "S", "W", "N"])); // Output: {x: 0, y: 1}
  ```

```
