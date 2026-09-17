# NumPy Hands-On Practice

From Python Lists to Numerical Computing

This repository contains my completed NumPy hands-on exercises and the Weather Temperature Analysis with NumPy mini project.

The work focuses on learning how to create NumPy arrays from Python lists, understand array dimensions and data types, perform element-wise numerical operations, and analyze simple temperature data.

---

# Project Overview

The exercises cover:

- Importing NumPy
- Creating NumPy arrays from Python lists
- Working with 1D arrays
- Working with 2D arrays
- Understanding vectors and matrices
- Inspecting array data types
- Comparing Python lists with NumPy arrays
- Performing element-wise calculations
- Analyzing temperature data
- Comparing temperatures between Lagos, Abuja, and Ibadan

---

# Hands-On 1 — Meet Your First NumPy Arrays

The first exercise introduced NumPy arrays using weather temperature data.

Topics Covered

- Importing NumPy
- Creating a NumPy array
- Identifying a 1D array
- Checking the array data type
- Creating a 2D array
- Understanding dimensions

Example Dataset

temperatures = [27.5, 29.0, 28.5]

The list was converted into a NumPy array:

temperature_array = np.array(temperatures)

The exercise also used a 2D weather dataset:

weather_data = [
    [27.5, 28.0, 29.5],
    [28.0, 29.0, 30.0]
]

This produced a 2D array, which can be described as a matrix with 2 rows and 3 values in each row.

---

# Hands-On 2 — Python Lists vs NumPy Arrays

The second exercise demonstrated the difference between Python lists and NumPy arrays when performing numerical operations.

Python Lists

sales_timothy = [10, 15, 20]
sales_brenda = [5, 10, 15]

print(sales_timothy + sales_brenda)

The result is:

[10, 15, 20, 5, 10, 15]

Python lists are combined rather than added element by element.

NumPy Arrays

sales_timothy_array = np.array(sales_timothy)
sales_brenda_array = np.array(sales_brenda)

print(sales_timothy_array + sales_brenda_array)

The result is:

[15 25 35]

This demonstrates that NumPy arrays allow arithmetic operations to be performed element by element.

---

# Mini Project — Weather Temperature Analysis with NumPy

### Project Introduction

This mini project analyzes temperature data recorded by a weather-monitoring station.

The project uses NumPy to convert numerical data into arrays and perform basic numerical analysis.

---

# Dataset

The weather station recorded the following temperatures for one week:

temperatures = [27.5, 29.0, 30.5, 28.0, 31.0, 32.5, 30.0]

The target temperatures were:

target = [28.0, 28.0, 29.0, 28.0, 30.0, 30.0, 29.0]

Three additional locations were also provided:

lagos = [27.5, 29.0, 30.5, 28.0, 31.0]

abuja = [25.0, 28.0, 29.5, 30.0, 32.0]

ibadan = [26.5, 28.5, 29.0, 27.5, 30.5]

---

# Array Inspection

The weekly temperature data was converted into a NumPy array.

temperature_array = np.array(temperatures)

The array was inspected using:

print(temperature_array.ndim)
print(temperature_array.dtype)
print(temperature_array.size)

Results

- Number of dimensions: 1
- Array type: Vector
- Data type: float64
- Number of observations: 7

---

➕ Numerical Operations

Temperature Difference

The recorded temperatures were compared with the target temperatures.

temperature_difference = temperature_array - target_array

print(temperature_difference)

Result:

[-0.5  1.   1.5  0.   1.   2.5  1. ]

A positive value means the recorded temperature was above the target, while a negative value means it was below the target.

---

Temperature Increase

The project also simulated an increase of 2°C:

increased_temperatures = temperature_array + 2

print(increased_temperatures)

Result:

[29.5 31.  32.5 30.  33.  34.5 32. ]

A "for" loop was not required because NumPy can perform the operation across the array.

---

# Lagos vs Abuja Comparison

The Lagos and Abuja arrays were compared using subtraction:

lagos_vs_abuja = lagos_array - abuja_array

print(lagos_vs_abuja)

Result:

[ 2.5  1.   1.  -2.  -1. ]

Interpretation

- Day 1: Lagos was 2.5°C higher than Abuja.
- Day 2: Lagos was 1.0°C higher than Abuja.
- Day 3: Lagos was 1.0°C higher than Abuja.
- Day 4: Abuja was 2.0°C higher than Lagos.
- Day 5: Abuja was 1.0°C higher than Lagos.

---

# Location Comparison

The three locations were compared to identify the highest temperature recorded on each day.

Results

Day| Location with Highest Temperature| Temperature
Day 1| Lagos| 27.5°C
Day 2| Lagos| 29.0°C
Day 3| Lagos| 30.5°C
Day 4| Abuja| 30.0°C
Day 5| Abuja| 32.0°C

---

# Temperature Increase by Location

Each location's temperatures were increased by 1°C.

lagos_plus_1 = lagos_array + 1
abuja_plus_1 = abuja_array + 1
ibadan_plus_1 = ibadan_array + 1

This demonstrated that NumPy can perform the same operation on every value in an array without manually processing each value.

---

# Findings

1. The highest recorded temperature during the week was 32.5°C on Day 6.

2. The recorded temperature was above the target temperature on Day 2, Day 3, Day 5, Day 6, and Day 7.

3. The recorded temperature was below the target temperature only on Day 1.

4. Lagos recorded the highest temperature on Days 1, 2, and 3 in the five-day location comparison.

5. Abuja recorded the highest temperature on Days 4 and 5.

---

# What I Learned

Through this project, I learned how to:

- Import NumPy using "import numpy as np"
- Convert Python lists into NumPy arrays
- Identify 1D and 2D arrays
- Understand vectors and matrices
- Inspect an array's data type using "dtype"
- Check the number of dimensions using "ndim"
- Check the number of values using "size"
- Perform element-wise addition and subtraction
- Perform calculations on an entire array
- Compare numerical datasets using NumPy
- Interpret numerical results rather than only displaying them

---

# Conclusion

This project provided practical experience with NumPy and numerical data.

The exercises demonstrated the difference between Python lists and NumPy arrays and showed how NumPy can make numerical calculations easier by performing operations element by element.

The Weather Temperature Analysis project also provided practice in analyzing temperature data and comparing values between different locations.

---

# Tools Used

- Python
- NumPy
- Jupyter Notebook

---

# Author

Owolabi Ayotomiwa Oluwafisayomi

This project was completed as part of Python/NumPy hands-on practice.
