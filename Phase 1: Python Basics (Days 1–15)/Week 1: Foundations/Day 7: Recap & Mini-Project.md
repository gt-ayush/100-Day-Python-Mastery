Let’s tackle **Day 7: Recap & Mini-Project**!  
Today, you’ll review concepts from Days 1–6 and build a **CLI Calculator** to solidify your understanding. 🧮  

---

### **Day 7: Recap & Mini-Project**  
**Objective**: Revise Python basics (variables, control flow, loops, functions) and build a functional calculator.  

---

#### **Step 1: Quick Recap**  
1. **Variables & Data Types**:  
   - Store numbers, strings, booleans.  
   - Type conversions (`int()`, `str()`, `float()`).  

2. **Control Flow**:  
   - `if-elif-else` for decision-making.  
   - Loops (`for`, `while`) with `break`/`continue`.  

3. **Functions**:  
   - Define reusable blocks with parameters and `return`.  

---

#### **Step 2: Mini-Project – CLI Calculator**  
**Requirements**:  
- Perform basic operations: **+**, **-**, **×**, **÷**.  
- Use functions for each operation.  
- Allow the user to input numbers and choose operations.  
- Handle invalid inputs (e.g., division by zero).  

---

##### **Step-by-Step Guide**  
1. **Define Arithmetic Functions**:  
   ```python  
   def add(a, b):  
       return a + b  

   def subtract(a, b):  
       return a - b  

   def multiply(a, b):  
       return a * b  

   def divide(a, b):  
       if b == 0:  
           return "Error: Division by zero!"  
       return a / b  
   ```  

2. **Create a Menu-Driven Interface**:  
   ```python  
   print("Calculator Menu:")  
   print("1. Add")  
   print("2. Subtract")  
   print("3. Multiply")  
   print("4. Divide")  
   print("5. Exit")  
   ```  

3. **Main Loop**:  
   ```python  
   while True:  
       choice = input("Enter choice (1-5): ")  

       if choice == "5":  
           print("Exiting calculator...")  
           break  

       num1 = float(input("Enter first number: "))  
       num2 = float(input("Enter second number: "))  

       if choice == "1":  
           print(f"Result: {add(num1, num2)}")  
       elif choice == "2":  
           print(f"Result: {subtract(num1, num2)}")  
       elif choice == "3":  
           print(f"Result: {multiply(num1, num2)}")  
       elif choice == "4":  
           print(f"Result: {divide(num1, num2)}")  
       else:  
           print("Invalid choice! Try again.")  
   ```  

---

#### **Step 3: Enhancements (Optional)**  
1. Add **exponentiation** (`a ** b`).  
2. Add a **history** feature to track previous calculations.  
3. Handle non-numeric inputs gracefully (use `try-except`).  

---

#### **Recap Questions**  
1. How do functions make this project easier to maintain?  
2. Why do we need `float(input(...))` instead of `input()` alone?  
3. What happens if the user enters `abc` instead of a number?  

---

#### **Challenge**  
Modify the calculator to support **multiple operations in a single run** (e.g., `3 + 5 * 2`).  
*(Hint: Parse the input string using `split()` and handle order of operations.)*  

---

**Your Task**:  
1. Build the calculator and share your code.  
2. Try adding at least one enhancement (e.g., exponentiation).  

Let me know if you get stuck or want feedback! 🚀
