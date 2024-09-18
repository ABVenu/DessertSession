### Student Notes:

# Advanced Mathematics and Conversions

### **1. Introduction**

Today’s focus is on advanced mathematical calculations and unit conversions. We will cover:

- Geometry and area calculations
- Volume calculations
- Temperature, distance, and volume conversions
- Discounts and compound interest
- Date and time calculations

### **2. Geometry and Area Calculations**

**Objective**: Learn to calculate the area of different geometric shapes.

#### **Rectangle**

- **Formula**: `Area = width × height`
- **Example**: For a rectangle with width = 5 units and height = 10 units:
  - Area = 5 × 10 = 50 square units

#### **Triangle**

- **Formula**: `Area = 0.5 × base × height`
- **Example**: For a triangle with base = 8 units and height = 6 units:
  - Area = 0.5 × 8 × 6 = 24 square units

#### **Circle**

- **Formula**: `Area = π × radius²`
- **Example**: For a circle with radius = 7 units:
  - Area = π × 7² ≈ 153.94 square units

**JavaScript Functions**:

```javascript
function calculateRectangleArea(width, height) {
  return width * height;
}

function calculateTriangleArea(base, height) {
  return 0.5 * base * height;
}

function calculateCircleArea(radius) {
  return Math.PI * radius * radius;
}
```

### **3. Volume Calculations**

**Objective**: Calculate the volume of common 3D shapes.

#### **Cube**

- **Formula**: `Volume = side³`
- **Example**: For a cube with side = 4 units:
  - Volume = 4³ = 64 cubic units

#### **Rectangular Prism**

- **Formula**: `Volume = length × width × height`
- **Example**: For a rectangular prism with length = 4 units, width = 5 units, height = 6 units:
  - Volume = 4 × 5 × 6 = 120 cubic units

#### **Sphere**

- **Formula**: `Volume = (4/3) × π × radius³`
- **Example**: For a sphere with radius = 3 units:
  - Volume = (4/3) × π × 3³ ≈ 113.1 cubic units

**JavaScript Functions**:

```javascript
function calculateCubeVolume(side) {
  return side * side * side;
}

function calculatePrismVolume(length, width, height) {
  return length * width * height;
}

function calculateSphereVolume(radius) {
  return (4 / 3) * Math.PI * Math.pow(radius, 3);
}
```

### **4. Conversions**

**Objective**: Perform conversions between different units.

#### **Temperature Conversions**

- **Celsius to Fahrenheit**:

  - **Formula**: `F = (C × 9/5) + 32`
  - **Example**: For Celsius = 25:
    - Fahrenheit = (25 × 9/5) + 32 = 77°F

- **Celsius to Kelvin**:
  - **Formula**: `K = C + 273.15`
  - **Example**: For Celsius = 25:
    - Kelvin = 25 + 273.15 = 298.15K

**JavaScript Functions**:

```javascript
function celsiusToFahrenheit(celsius) {
  return (celsius * 9) / 5 + 32;
}

function celsiusToKelvin(celsius) {
  return celsius + 273.15;
}
```

#### **Distance Conversions**

- **Meters to Kilometers**:
  - **Formula**: `Km = M / 1000`
  - **Example**: For meters = 1500:
    - Kilometers = 1500 / 1000 = 1.5 km

**JavaScript Function**:

```javascript
function metersToKilometers(meters) {
  return meters / 1000;
}
```

#### **Volume Conversions**

- **Liters to Milliliters**:
  - **Formula**: `Ml = L × 1000`
  - **Example**: For liters = 2:
    - Milliliters = 2 × 1000 = 2000 ml

**JavaScript Function**:

```javascript
function litersToMilliliters(liters) {
  return liters * 1000;
}
```

### **5. Discounts and Advanced Calculations**

**Objective**: Solve real-world problems involving discounts and compound interest.

#### **Discount Calculation**

- **Formula**: `Final Price = Original Price × (1 - Discount Percentage)`
- **Example**: For Original Price = $100 and Discount Percentage = 20%:
  - Final Price = 100 × (1 - 0.20) = $80

**JavaScript Function**:

```javascript
function calculateDiscountedPrice(originalPrice, discountPercentage) {
  return originalPrice * (1 - discountPercentage / 100);
}
```

#### **Compound Interest Calculation**

- **Formula**: `Amount = Principal × (1 + Rate/100) ^ Time`
- **Example**: For Principal = $1000, Rate = 5%, Time = 2 years:
  - Amount = 1000 × (1 + 0.05)² ≈ $1102.50

**JavaScript Function**:

```javascript
function calculateCompoundInterest(principal, rate, time) {
  return principal * Math.pow(1 + rate / 100, time);
}
```

### **6. Date and Time Calculations**

**Objective**: Use JavaScript to handle date and time calculations.

#### **Current Date and Time**

- **JavaScript**: `new Date()`
- **Example**: `new Date()` returns the current date and time.

#### **Difference Between Dates**

- **Formula**: `(new Date("YYYY-MM-DD") - new Date("YYYY-MM-DD")) / (1000 * 60 * 60 * 24)`
- **Example**: Difference between "2024-09-01" and "2024-08-01":
  - Difference = (new Date("2024-09-01") - new Date("2024-08-01")) / (1000 _ 60 _ 60 \* 24) = 31 days

**JavaScript Function**:

```javascript
function calculateDateDifference(date1, date2) {
  const diffTime = Math.abs(new Date(date1) - new Date(date2));
  return Math.ceil(diffTime / (1000 * 60 * 60 * 24));
}
```

#### **Formatting Dates and Times**

- **JavaScript**: `date.toLocaleDateString()`, `date.toLocaleTimeString()`
- **Example**: `new Date().toLocaleDateString()` returns "09/18/2024", `new Date().toLocaleTimeString()` returns "10:30:00 AM"

**JavaScript Functions**:

```javascript
function formatDate(date) {
  return date.toLocaleDateString();
}

function formatTime(date) {
  return date.toLocaleTimeString();
}
```

### **7. Wrap-Up and Q&A**

- **Summary**: Review the formulas and JavaScript functions learned today.
- **Q&A**: Address any questions or clarifications needed.

### **8. Assignment**

**Objective**: Reinforce today’s learning with practice problems.

- **Instructions**: Complete the assignment to practice advanced mathematical calculations and conversions.

---
