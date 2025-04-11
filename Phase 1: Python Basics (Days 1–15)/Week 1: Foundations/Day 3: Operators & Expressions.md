Let’s dive into **Day 3: Operators & Expressions**!  
You’ll learn to perform calculations, compare values, and combine conditions. 🔢  

---

### **Day 3: Operators & Expressions**  
**Objective**: Master arithmetic, comparison, and logical operators.  

---

#### **Step 1: Arithmetic Operators**  
Perform mathematical operations:  
| Operator | Description      | Example         | Result  |  
|----------|------------------|-----------------|---------|  
| `+`      | Addition         | `5 + 3`         | `8`     |  
| `-`      | Subtraction      | `10 - 2.5`      | `7.5`   |  
| `*`      | Multiplication   | `4 * 3`         | `12`    |  
| `/`      | Division         | `10 / 3`        | `3.333` |  
| `%`      | Modulus (remainder) | `10 % 3`    | `1`     |  
| `**`     | Exponentiation   | `2 ** 3`        | `8`     |  
| `//`     | Floor division   | `10 // 3`       | `3`     |  

**Example**:  
```python  
x = 10  
y = 3  
print(x // y)  # Output: 3 (floor division ignores decimal)  
```  

---

#### **Step 2: Comparison Operators**  
Compare values and return `True`/`False`:  
| Operator | Description          | Example       | Result  |  
|----------|----------------------|---------------|---------|  
| `==`     | Equal to             | `5 == 5`      | `True`  |  
| `!=`     | Not equal to         | `5 != 3`      | `True`  |  
| `>`      | Greater than         | `10 > 5`      | `True`  |  
| `<`      | Less than            | `10 < 5`      | `False` |  
| `>=`     | Greater than or equal| `10 >= 10`    | `True`  |  
| `<=`     | Less than or equal   | `5 <= 3`      | `False` |  

**Example**:  
```python  
age = 20  
print(age >= 18)  # Output: True (eligible to vote)  
```  

---

#### **Step 3: Logical Operators**  
Combine conditions using `and`, `or`, `not`:  

| Operator | Description                          | Example                   | Result  |  
|----------|--------------------------------------|---------------------------|---------|  
| `and`    | True if **both** are true            | `(5 > 3) and (2 < 1)`     | `False` |  
| `or`     | True if **at least one** is true     | `(5 > 3) or (2 < 1)`      | `True`  |  
| `not`    | Inverts the result                   | `not (5 > 3)`             | `False` |  

**Example**:  
```python  
is_weekend = True  
has_money = False  
print(is_weekend and has_money)  # Output: False (can’t party 😢)  
```  

---

#### **Step 4: Expressions**  
Combine variables, operators, and values:  
```python  
# Calculate area of a circle  
radius = 5  
area = 3.14 * (radius ** 2)  
print(f"Area: {area}")  # Output: Area: 78.5  
```  

---

### **Coding Exercises**  
1. **Basic Calculator**:  
   - Ask the user for two numbers and print:  
     - Sum, difference, product, and quotient.  
   ```python  
   num1 = float(input("Enter first number: "))  
   num2 = float(input("Enter second number: "))  
   print(f"Sum: {num1 + num2}")  
   print(f"Product: {num1 * num2}")  
   ```  

2. **Comparison Challenge**:  
   - Check if a number is even **and** positive.  
   ```python  
   num = int(input("Enter a number: "))  
   is_even_positive = (num % 2 == 0) and (num > 0)  
   print(f"Result: {is_even_positive}")  
   ```  

3. **Logical Puzzle**:  
   - A movie ticket is free if age ≤ 12 **or** age ≥ 60. Write a program to check eligibility.  
   ```python  
   age = int(input("Enter your age: "))  
   is_free = (age <= 12) or (age >= 60)  
   print(f"Free ticket: {is_free}")  
   ```  

---

#### **Recap Questions**  
1. What’s the result of `2 ** 3 + 10 % 3`?  
2. Why does `print(5 == "5")` return `False`?  
3. Simplify: `not (x > 5 and y < 10)` using De Morgan’s Law.  

---

#### **What’s Next?**  
Tomorrow: **Control Flow (Part 1)** – `if-elif-else` statements!  

---

**Your Task**:  
1. Share your code for the exercises.  
2. Try mixing operators (e.g., `(5 + 3) * (10 - 2)`).  

Let me know if you need help! 😊
