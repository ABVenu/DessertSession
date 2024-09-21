#### Student Notes

# Logical Reasoning using JavaScript

#### **1. Introduction to Logical Reasoning in JavaScript**

- **Overview:**  
  Logical reasoning in programming involves making decisions based on conditions and solving problems systematically. In JavaScript, this is achieved through conditionals (e.g., `if-else` statements) and loops.

- **Example:**  
  Use `if-else` to decide between transportation options:
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

- **Explanation:**  
  Encoding converts data into a format suitable for transmission or storage, while decoding reverses the process. Common types include Base64 encoding for secure data and URL encoding for safe URL transmission.

- **Example:**  
  Base64 encoding and decoding in JavaScript:

  ```javascript
  let encoded = btoa("Hello World!"); // Base64 encode
  let decoded = atob(encoded); // Base64 decode
  console.log(encoded); // Output: "SGVsbG8gV29ybGQh"
  console.log(decoded); // Output: "Hello World!"
  ```

- **Exercise:**  
  Create functions to encode and decode strings, handling data for secure transmission or URL handling.

#### **3. Cipher and Decipher Strings**

- **Explanation:**  
  A cipher is a method to transform text into an unreadable format to secure it. The Caesar cipher shifts letters by a certain number of positions in the alphabet.

- **JavaScript Example (Caesar Cipher):**

  **Cipher Function:**

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

  **Decipher Function:**

  ```javascript
  function decipher(str, shift) {
    return cipher(str, 26 - shift); // Reverse the cipher shift
  }
  console.log(decipher("khoor", 3)); // Output: "hello"
  ```

- **Exercise:**  
  Implement cipher and decipher functions to encode and decode messages using different shift values.

#### **4. Data Sufficiency**

- **Explanation:**  
  Data sufficiency determines if enough data is available to solve a problem. This is useful in scenarios like form validation where certain data must be present.

- **JavaScript Example:**

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

- **Exercise:**  
  Write functions to check if sufficient data is provided to solve problems like calculating volumes or prices.

#### **5. Clocks and Calendars (with Date Function)**

- **Explanation:**  
  The JavaScript `Date` object helps handle date and time operations, such as calculating differences between dates and converting time zones.

- **JavaScript Example:**

  ```javascript
  function daysBetween(date1, date2) {
    let diffInTime = new Date(date2) - new Date(date1);
    let diffInDays = diffInTime / (1000 * 3600 * 24);
    return Math.abs(diffInDays);
  }
  console.log(daysBetween("2024-09-18", "2024-09-25")); // Output: 7
  ```

- **Exercise:**  
  Calculate the difference between two dates, find deadlines, or convert between time zones using the `Date` object.

#### **6. Boolean Algebra**

- **Explanation:**  
  Boolean algebra involves logical operations using true/false values. It is crucial for form validation and access control, checking if multiple conditions are met.

- **JavaScript Example:**

  ```javascript
  function isEligible(age, hasLicense) {
    return age >= 18 && hasLicense;
  }
  console.log(isEligible(19, true)); // Output: true
  console.log(isEligible(17, true)); // Output: false
  ```

- **Exercise:**  
  Create functions to validate data by combining multiple conditions using Boolean operators.

#### **7. Directions**

- **Explanation:**  
  Directions involve calculating positions based on movement (North, South, East, West). This is useful in navigation and tracking systems.

- **JavaScript Example:**

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

- **Exercise:**  
  Build a function to simulate navigation based on a series of directional moves.

#### **8. Practical Application Review**

- **Review:**  
  Discuss how encoding/decoding, cipher/decipher, Boolean logic, date/time management, and directional logic apply to real-world applications such as web apps and games.

#### **9. Q&A and Wrap-Up**

- **Open Discussion:**  
  Address any questions and clarify concepts covered in the session.

- **Homework Exercise:**  
  Assign a brief exercise to reinforce the concepts learned during the session.

---
