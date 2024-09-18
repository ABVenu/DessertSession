# Logical Reasoning using JavaScript-II

#### Submission Guidelines

## **Please Solve all the question in a single file on One Compiler [Link](https://onecompiler.com/javascript), Save it with proper naming, Run It and Submit the One Complier Link, Please Ensure Code visiblity is Public**

### **1. Data Sufficiency for Rectangle Perimeter**

Write a function that takes the length and width of a rectangle as input and determines if there is sufficient data to calculate the perimeter.

- **Input 1**: `5`, `4`  
  **Output 1**: `"Sufficient data. Perimeter: 18"`

- **Input 2**: `null`, `10`  
  **Output 2**: `"Insufficient data"` (Edge case: missing length)

- **Input 3**: `7`, `0`  
  **Output 3**: `"Insufficient data"` (Edge case: zero width)

- **Input 4**: `9`, `6`  
  **Output 4**: `"Sufficient data. Perimeter: 30"`

- **Input 5**: `8`, `null`  
  **Output 5**: `"Insufficient data"` (Edge case: missing width)

---

### **2. Calculate Number of Days Between Two Dates**

Write a function that takes two date strings (in `YYYY-MM-DD` format) and returns the number of days between them.

- **Input 1**: `"2024-01-01"`, `"2024-01-10"`  
  **Output 1**: `9`

- **Input 2**: `"2024-12-31"`, `"2025-01-01"`  
  **Output 2**: `1` (Edge case: year boundary)

- **Input 3**: `"2024-02-28"`, `"2024-03-01"`  
  **Output 3**: `2` (Edge case: leap year)

- **Input 4**: `"2023-09-18"`, `"2024-09-18"`  
  **Output 4**: `366` (Edge case: leap year)

- **Input 5**: `"2024-09-18"`, `"2024-09-10"`  
  **Output 5**: `8` (Edge case: date order reversed)

---

### **3. Convert Date to Day of the Week**

Write a function that takes a date string in the format `YYYY-MM-DD` and returns the day of the week for that date.

- **Input 1**: `"2024-01-01"`  
  **Output 1**: `"Monday"`

- **Input 2**: `"2024-09-18"`  
  **Output 2**: `"Wednesday"`

- **Input 3**: `"2023-12-25"`  
  **Output 3**: `"Monday"`

- **Input 4**: `"2025-07-04"`  
  **Output 4**: `"Friday"`

- **Input 5**: `"2022-02-28"`  
  **Output 5**: `"Monday"`

---

### **4. Boolean Algebra: AND Operation**

Write a function that performs an AND operation between two boolean values.

- **Input 1**: `true`, `true`  
  **Output 1**: `true`

- **Input 2**: `true`, `false`  
  **Output 2**: `false`

- **Input 3**: `false`, `false`  
  **Output 3**: `false`

- **Input 4**: `false`, `true`  
  **Output 4**: `false`

- **Input 5**: `true`, `true`  
  **Output 5**: `true`

---

### **5. Boolean Algebra: OR Operation**

Write a function that performs an OR operation between two boolean values.

- **Input 1**: `true`, `true`  
  **Output 1**: `true`

- **Input 2**: `true`, `false`  
  **Output 2**: `true`

- **Input 3**: `false`, `false`  
  **Output 3**: `false`

- **Input 4**: `false`, `true`  
  **Output 4**: `true`

- **Input 5**: `false`, `false`  
  **Output 5**: `false`

---

### **6. Determine Direction Facing After Turns**

Write a function that simulates turning left or right from an initial direction (north, east, south, west) and returns the final direction.

- **Input 1**: `"north"`, `"left"`  
  **Output 1**: `"west"`

- **Input 2**: `"east"`, `"right"`  
  **Output 2**: `"south"`

- **Input 3**: `"south"`, `"left"`  
  **Output 3**: `"east"`

- **Input 4**: `"west"`, `"right"`  
  **Output 4**: `"north"`

- **Input 5**: `"north"`, `"right"`  
  **Output 5**: `"east"`

---
