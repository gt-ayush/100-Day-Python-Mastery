Let’s dive into **Day 6: Functions (Basics)**!  
Today, you’ll learn to write reusable blocks of code using functions. 🛠️  

---

### **Day 6: Functions (Basics)**  
**Objective**: Define functions, use parameters, and return values.  

---

#### **Step 1: What is a Function?**  
- A **function** is a named block of code that performs a specific task.  
- **Why use functions?**  
  - Reuse code (avoid repetition).  
  - Organize logic into modular pieces.  

**Syntax**:  
```python  
def function_name(parameters):  
    # code to execute  
    return result  # optional  
```  

---

#### **Step 2: Defining & Calling Functions**  
1. **Define a function**:  
   ```python  
   def greet():  
       print("Hello! Welcome to Python.")  
   ```  

2. **Call the function**:  
   ```python  
   greet()  # Output: Hello! Welcome to Python.  
   ```  

---

#### **Step 3: Parameters & Arguments**  
- **Parameters**: Variables listed in the function definition.  
- **Arguments**: Actual values passed to the function.  

**Example**:  
```python  
def add(a, b):  # a and b are parameters  
    return a + b  

result = add(2, 3)  # 2 and 3 are arguments  
print(result)  # Output: 5  
```  

---

#### **Step 4: Return Statement**  
- `return` sends a value back to the caller.  
- A function without `return` defaults to `None`.  

**Example**:  
```python  
def is_even(num):  
    return num % 2 == 0  

print(is_even(4))  # Output: True  
```  

---

#### **Step 5: Scope of Variables**  
- **Local variables**: Defined inside a function (not accessible outside).  
- **Global variables**: Defined outside functions (accessible everywhere).  

**Example**:  
```python  
x = 10  # Global  

def my_func():  
    y = 5  # Local  
    print(x + y)  

my_func()  # Output: 15  
print(y)   # Error: y is not defined  
```  

---

### **Coding Exercises**  
1. **Basic Function**:  
   Write a function `calculate_area(radius)` that returns the area of a circle.  
   ```python  
   def calculate_area(radius):  
       return 3.14 * (radius ** 2)  
   print(calculate_area(5))  # Output: 78.5  
   ```  

2. **Temperature Converter**:  
   Create a function `celsius_to_fahrenheit(c)` that converts Celsius to Fahrenheit.  
   Formula: `F = (C * 9/5) + 32`  

3. **String Reverser**:  
   Write a function `reverse_string(s)` that returns the reversed version of a string.  
   ```python  
   reverse_string("hello")  # Output: "olleh"  
   ```  

4. **Challenge (Prime Checker)**:  
   Create a function `is_prime(n)` that returns `True` if `n` is a prime number.  

---

#### **Common Mistakes**  
- Forgetting `()` when calling a function.  
- Mixing up **parameters** (defined) and **arguments** (passed).  
- Modifying global variables without `global` keyword.  

---

#### **Recap Questions**  
1. What’s the difference between `print()` and `return`?  
2. How many values can a function return?  
3. What happens if you call `add(2)` instead of `add(2, 3)`?  

---

#### **What’s Next?**  
Tomorrow: **Day 7: Recap & Mini-Project** – Build a CLI calculator using functions!  

---

**Your Task**:  
1. Share your code for the exercises (especially the prime checker!).  
2. Write a function `greet(name)` that takes a default parameter `name="User"`.  

Let me know if you need hints! 😊
