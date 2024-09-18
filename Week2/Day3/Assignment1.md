# Logical Reasoning using JavaScript-I

#### Submission Guidelines

## **Please Solve all the question in a single file on One Compiler [Link](https://onecompiler.com/javascript), Save it with proper naming, Run It and Submit the One Complier Link, Please Ensure Code visiblity is Public**

### **1. Encode a String in Base64**

Write a function that takes a string as input and returns the Base64 encoded version of it.

- **Input 1**: `"Good Morning"`  
  **Output 1**: `"R29vZCBNb3JuaW5n"`

- **Input 2**: `"JavaScript is awesome!"`  
  **Output 2**: `"SmF2YVNjcmlwdCBpcyBhd2Vzb21lIQ=="`

- **Input 3**: `""`  
  **Output 3**: `""` (Edge case: empty string)

- **Input 4**: `" "`  
  **Output 4**: `"IA=="` (Edge case: single space)

- **Input 5**: `"Encode123!"`  
  **Output 5**: `"RW5jb2RlMTIzIQ=="`

---

### **2. Decode a Base64 String**

Write a function that decodes a Base64 encoded string back to its original string form.

- **Input 1**: `"U2ltcGxlIFRleHQ="`  
  **Output 1**: `"Simple Text"`

- **Input 2**: `"T25lIFJvY2s="`  
  **Output 2**: `"One Rock"`

- **Input 3**: `"SmF2YVNjcmlwdCBNYWdpYw=="`  
  **Output 3**: `"JavaScript Magic"`

- **Input 4**: `""`  
  **Output 4**: `""` (Edge case: empty string)

- **Input 5**: `"c2VjcmV0=="`  
  **Output 5**: `"secret"`

---

### **3. Cipher a String (Caesar Cipher)**

Write a function that takes a string and an integer shift value, and returns the string encrypted using a Caesar Cipher.

- **Input 1**: `"abc"`, `3`  
  **Output 1**: `"def"`

- **Input 2**: `"open"`, `2`  
  **Output 2**: `"qrgo"`

- **Input 3**: `"xyz"`, `5`  
  **Output 3**: `"cde"` (Edge case: wrap-around alphabet)

- **Input 4**: `"HELLO"`, `4`  
  **Output 4**: `"LIPPS"` (Edge case: uppercase letters)

- **Input 5**: `"pass123"`, `3`  
  **Output 5**: `"sdvv123"` (Edge case: digits remain unchanged)

---

### **4. Decipher a String (Caesar Cipher)**

Write a function that takes a Caesar Cipher encrypted string and an integer shift value, and returns the original string.

- **Input 1**: `"def"`, `3`  
  **Output 1**: `"abc"`

- **Input 2**: `"qrgo"`, `2`  
  **Output 2**: `"open"`

- **Input 3**: `"cde"`, `5`  
  **Output 3**: `"xyz"` (Edge case: wrap-around alphabet)

- **Input 4**: `"LIPPS"`, `4`  
  **Output 4**: `"HELLO"` (Edge case: uppercase letters)

- **Input 5**: `"sdvv123"`, `3`  
  **Output 5**: `"pass123"` (Edge case: digits remain unchanged)

---

### **5. Data Sufficiency for Calculating Circle Area**

Write a function that takes the radius of a circle as input and returns whether there’s sufficient data to calculate the area.

- **Input 1**: `7`  
  **Output 1**: `"Sufficient data. Area: 153.94"`

- **Input 2**: `0`  
  **Output 2**: `"Insufficient data"` (Edge case: radius is zero)

- **Input 3**: `null`  
  **Output 3**: `"Insufficient data"` (Edge case: missing radius)

- **Input 4**: `10`  
  **Output 4**: `"Sufficient data. Area: 314.16"`

- **Input 5**: `-5`  
  **Output 5**: `"Insufficient data"` (Edge case: negative radius)

---