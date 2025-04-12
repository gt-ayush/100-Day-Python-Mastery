Let’s dive into **Day 5: Control Flow (Part 2)**!  
Today, you’ll master loops (`for` and `while`) and control them with `break` and `continue`. 🔄  

---

### **Day 5: Control Flow (Part 2)**  
**Objective**: Use loops to automate repetitive tasks and control their flow.  

---

#### **Step 1: `for` Loops**  
- **Syntax**: Iterate over sequences (lists, strings, ranges, etc.).  
  ```python  
  for item in sequence:  
      # code to repeat  
  ```  
- **Example**:  
  ```python  
  fruits = ["apple", "banana", "cherry"]  
  for fruit in fruits:  
      print(f"I love {fruit}!")  
  ```  
  **Output**:  
  ```  
  I love apple!  
  I love banana!  
  I love cherry!  
  ```  

---

#### **Step 2: `range()` Function**  
- Generate a sequence of numbers:  
  - `range(stop)`: `0` to `stop-1`  
  - `range(start, stop)`  
  - `range(start, stop, step)`  
- **Example**:  
  ```python  
  for num in range(1, 6):  
      print(num)  # Output: 1 2 3 4 5  
  ```  

---

#### **Step 3: `while` Loops**  
- **Syntax**: Repeat code **while** a condition is `True`.  
  ```python  
  while condition:  
      # code to repeat  
  ```  
- **Example** (Countdown):  
  ```python  
  count = 5  
  while count > 0:  
      print(count)  
      count -= 1  # Decrement count by 1  
  print("Blastoff!")  
  ```  
  **Output**:  
  ```  
  5  
  4  
  3  
  2  
  1  
  Blastoff!  
  ```  

---

#### **Step 4: `break` and `continue`**  
- `break`: Exit the loop immediately.  
- `continue`: Skip the rest of the current iteration.  

**Example** (Search with `break`):  
```python  
fruits = ["apple", "banana", "cherry"]  
for fruit in fruits:  
    if fruit == "banana":  
        print("Found banana!")  
        break  
```  

**Example** (Skip even numbers with `continue`):  
```python  
for num in range(10):  
    if num % 2 == 0:  
        continue  # Skip even numbers  
    print(num)  # Output: 1 3 5 7 9  
```  

---

### **Coding Exercises**  
1. **Sum Numbers**:  
   Use a `for` loop to calculate the sum of numbers from 1 to 100.  
   ```python  
   total = 0  
   for num in range(1, 101):  
       total += num  
   print(f"Sum: {total}")  # Output: 5050  
   ```  

2. **Guessing Game**:  
   Use a `while` loop to let the user guess a secret number (e.g., `7`).  
   ```python  
   secret = 7  
   while True:  
       guess = int(input("Guess a number (1-10): "))  
       if guess == secret:  
           print("You won!")  
           break  
       else:  
           print("Try again!")  
   ```  

3. **Odd Numbers**:  
   Print all odd numbers between 1 and 20 using `continue`.  

4. **Challenge (Fibonacci)**:  
   Generate the first 10 Fibonacci numbers using a loop.  
   ```python  
   a, b = 0, 1  
   for _ in range(10):  
       print(a, end=" ")  
       a, b = b, a + b  
   # Output: 0 1 1 2 3 5 8 13 21 34  
   ```  

---

#### **Common Mistakes**  
- Infinite `while` loops (forget to update the condition).  
- Using `=` instead of `==` in conditions.  
- Forgetting the colon `:` after loop declarations.  

---

#### **Recap Questions**  
1. How does `range(5)` differ from `range(1, 5)`?  
2. What happens if you forget `count -= 1` in the countdown example?  
3. How would you print numbers from 10 to 1 using `range()`?  

---

#### **What’s Next?**  
Tomorrow: **Functions (Basics)** – Learn to write reusable blocks of code!  

---

**Your Task**:  
1. Share your code for the exercises.  
2. Modify the Fibonacci code to ask the user how many terms to generate.  

Let me know if you need help debugging! 😊
