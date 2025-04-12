Let’s dive into **Day 4: Control Flow (Part 1)**!  
Today, you’ll learn to make decisions in your code using `if`, `elif`, and `else`. 🧠  

---

### **Day 4: Control Flow (Part 1)**  
**Objective**: Use conditional statements (`if-elif-else`) to create logic-based programs.  

---

#### **Step 1: The `if` Statement**  
- **Syntax**:  
  ```python  
  if condition:  
      # code to execute if condition is True  
  ```  
- **Example**:  
  ```python  
  age = 18  
  if age >= 18:  
      print("You can vote!")  
  ```  

---

#### **Step 2: The `else` Statement**  
- **Syntax**:  
  ```python  
  if condition:  
      # code if True  
  else:  
      # code if False  
  ```  
- **Example**:  
  ```python  
  num = 10  
  if num % 2 == 0:  
      print("Even")  
  else:  
      print("Odd")  
  ```  

---

#### **Step 3: The `elif` Statement**  
- **Syntax**:  
  ```python  
  if condition1:  
      # code  
  elif condition2:  
      # code  
  else:  
      # code  
  ```  
- **Example** (Grade Checker):  
  ```python  
  score = 85  
  if score >= 90:  
      print("A")  
  elif score >= 80:  
      print("B")  
  elif score >= 70:  
      print("C")  
  else:  
      print("Fail")  
  ```  

---

#### **Step 4: Nested Conditionals**  
- **Example** (Login System):  
  ```python  
  username = "admin"  
  password = "1234"  
  if username == "admin":  
      if password == "1234":  
          print("Login successful!")  
      else:  
          print("Wrong password!")  
  else:  
      print("Invalid username!")  
  ```  

---

### **Coding Exercises**  
1. **Basic Check**:  
   - Write a program to check if a number is positive, negative, or zero.  
   ```python  
   num = float(input("Enter a number: "))  
   if num > 0:  
       print("Positive")  
   elif num < 0:  
       print("Negative")  
   else:  
       print("Zero")  
   ```  

2. **Grade Calculator**:  
   - Convert a score (0-100) to a letter grade (A/B/C/D/F).  

3. **Login System**:  
   - Ask the user for a username and password.  
   - Check if they match predefined values (e.g., `user="alice"`, `password="python"`).  

4. **Challenge (Leap Year)**:  
   - A year is a leap year if:  
     - Divisible by 4 **but not** by 100 **unless** also divisible by 400.  
   ```python  
   year = int(input("Enter a year: "))  
   if (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0):  
       print("Leap year!")  
   else:  
       print("Not a leap year.")  
   ```  

---

#### **Common Mistakes**  
1. Forgetting the colon `:` after `if`, `elif`, or `else`.  
2. Incorrect indentation (use 4 spaces or a tab).  
3. Using `=` (assignment) instead of `==` (comparison).  

---

#### **Recap Questions**  
1. What’s wrong with this code?  
   ```python  
   if 5 > 3  
       print("True")  
   ```  
2. Why does `elif` come after `if` and before `else`?  
3. How would you check if a number is **either** 5 **or** 10?  

---

#### **What’s Next?**  
Tomorrow: **Control Flow (Part 2)** – `for` and `while` loops!  

---

**Your Task**:  
1. Complete the exercises (share your code).  
2. Try adding more conditions to the leap year problem (e.g., invalid year < 0).  

Let me know if you need help! 😊
