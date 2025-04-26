Let’s dive into **Day 11: Error Handling**!  
Today, you’ll learn to gracefully handle errors and exceptions in your code using `try`-`except` blocks. 🛡️  

---

### **Day 11: Error Handling**  
**Objective**: Use `try`-`except`-`else`-`finally` blocks to catch and manage exceptions.  

---

#### **Step 1: What Are Exceptions?**  
- **Exceptions** are errors that occur during program execution (e.g., division by zero, invalid input).  
- Without handling them, your program crashes.  

**Common Exceptions**:  
- `ValueError`: Invalid input (e.g., `int("abc")`).  
- `IndexError`: Accessing a non-existent list index.  
- `KeyError`: Accessing a missing dictionary key.  
- `ZeroDivisionError`: Dividing by zero.  

---

#### **Step 2: Basic `try`-`except` Block**  
Catch and handle exceptions to prevent crashes.  

**Syntax**:  
```python  
try:  
    # Risky code  
except ExceptionType:  
    # Handle the error  
```  

**Example**:  
```python  
try:  
    num = int(input("Enter a number: "))  
except ValueError:  
    print("Invalid input! Please enter a number.")  
```  

---

#### **Step 3: Handling Multiple Exceptions**  
Catch different errors with separate `except` blocks.  

**Example**:  
```python  
try:  
    num = int(input("Enter a number: "))  
    result = 10 / num  
    print(f"Result: {result}")  
except ValueError:  
    print("Invalid input! Not a number.")  
except ZeroDivisionError:  
    print("Cannot divide by zero!")  
```  

---

#### **Step 4: `else` and `finally` Clauses**  
- **`else`**: Runs if no exceptions occur.  
- **`finally`**: Always runs, regardless of exceptions (e.g., cleanup tasks).  

**Example**:  
```python  
try:  
    file = open("data.txt", "r")  
except FileNotFoundError:  
    print("File not found!")  
else:  
    print(file.read())  
    file.close()  
finally:  
    print("Execution complete.")  
```  

---

#### **Step 5: Raising Exceptions**  
Force an error with `raise` (e.g., validate input).  

**Example**:  
```python  
age = int(input("Enter your age: "))  
if age < 0:  
    raise ValueError("Age cannot be negative!")  
```  

---

#### **Step 6: Custom Exceptions**  
Create your own exception classes (optional but powerful).  

**Example**:  
```python  
class NegativeNumberError(Exception):  
    pass  # Inherits from base Exception class  

def sqrt(x):  
    if x < 0:  
        raise NegativeNumberError("Negative numbers not allowed!")  
    return x ** 0.5  

try:  
    print(sqrt(-5))  
except NegativeNumberError as e:  
    print(e)  
```  

---

### **Coding Exercises**  
1. **Safe Division**:  
   Ask for two numbers and handle division by zero.  
   ```python  
   try:  
       a = float(input("Enter numerator: "))  
       b = float(input("Enter denominator: "))  
       print(a / b)  
   except ZeroDivisionError:  
       print("Cannot divide by zero!")  
   except ValueError:  
       print("Invalid input!")  
   ```  

2. **List Access Guard**:  
   Handle `IndexError` when accessing a list.  
   ```python  
   my_list = [10, 20, 30]  
   try:  
       print(my_list[5])  
   except IndexError:  
       print("Index out of bounds!")  
   ```  

3. **Password Validator**:  
   Raise an error if a password is less than 8 characters.  
   ```python  
   password = input("Enter password: ")  
   if len(password) < 8:  
       raise ValueError("Password must be at least 8 characters!")  
   ```  

4. **Challenge (Retry Loop)**:  
   Keep asking for input until the user enters a valid number.  
   ```python  
   while True:  
       try:  
           num = int(input("Enter a number: "))  
           break  
       except ValueError:  
           print("Invalid input. Try again!")  
   ```  

---

#### **Recap Questions**  
1. What’s the difference between `ValueError` and `TypeError`?  
2. When would you use `finally` instead of `else`?  
3. Why is it bad practice to use a bare `except:` (without specifying the exception)?  

---

#### **Common Mistakes**  
- Catching too broad an exception (e.g., `except Exception` hides bugs).  
- Forgetting to close resources (files, network connections) in `finally`.  
- Overusing exceptions for control flow (use `if` checks when possible).  

---

#### **What’s Next?**  
Tomorrow: **Day 12: File Handling** – Read/write files and work with CSV/JSON!  

---

**Your Task**:  
1. Share your code for the exercises.  
2. Extend the password validator to check for uppercase letters and symbols.  

Let me know if you need help debugging! 😊
