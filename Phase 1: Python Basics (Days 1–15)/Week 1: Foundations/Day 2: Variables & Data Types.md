Got it! Let’s dive into **Day 2: Variables & Data Types**.  
You’ll learn to store and manipulate different kinds of data. 💡  

---

### **Day 2: Variables & Data Types**  
**Objective**: Understand variables, basic data types (integers, floats, strings, booleans), and type conversion.  

---

#### **Step 1: Variables**  
- **Variables** are containers for storing data.  
- **Rules for naming**:  
  - Start with a letter or `_`.  
  - Cannot start with a number or special character.  
  - Case-sensitive (`age` ≠ `Age`).  

**Example**:  
```python  
name = "Alice"  
age = 25  
height = 5.6  
is_student = True  
```  

---

#### **Step 2: Data Types**  
1. **Integers**: Whole numbers (`10`, `-5`, `2024`).  
2. **Floats**: Decimal numbers (`3.14`, `-0.99`).  
3. **Strings**: Text enclosed in quotes (`"Hello"`, `'Python'`).  
4. **Booleans**: `True` or `False`.  

**Check a variable’s type**:  
```python  
print(type(age))      # Output: <class 'int'>  
print(type(is_student)) # Output: <class 'bool'>  
```  

---

#### **Step 3: Type Conversion**  
Convert between types using:  
- `int()`: Converts to integer.  
- `float()`: Converts to float.  
- `str()`: Converts to string.  

**Example**:  
```python  
num_str = "123"  
num_int = int(num_str)  # Converts string "123" to integer 123  
```  

---

#### **Coding Exercises**  
1. **Basic Variables**:  
   Create variables for:  
   - Your favorite book (string).  
   - Your birth year (integer).  
   - Your height (float).  
   - Whether you like Python (boolean).  

2. **Type Conversion**:  
   - Ask the user for their age using `input()` (returns a string).  
   - Convert it to an integer and calculate their birth year.  
   ```python  
   age = input("Enter your age: ")  
   birth_year = 2024 - int(age)  
   print(f"You were born in {birth_year}.")  
   ```  

3. **Challenge**:  
   Write a program to add two numbers entered by the user.  
   ```python  
   num1 = float(input("Enter first number: "))  
   num2 = float(input("Enter second number: "))  
   print(f"Sum: {num1 + num2}")  
   ```  

---

#### **Recap Questions**  
1. What’s the difference between `"5"` (string) and `5` (integer)?  
2. Why does `print(10 + "5")` throw an error? How to fix it?  
3. How would you convert `3.9` to an integer? What’s the result?  

---

#### **What’s Next?**  
Tomorrow: **Operators & Expressions** (arithmetic, comparison, and logical operations).  

---

**Your Task**:  
1. Complete the exercises and share your code.  
2. Experiment with type conversions (e.g., `str(3.14) + " is pi"`).  

Let me know if you get stuck or want feedback! 😊
