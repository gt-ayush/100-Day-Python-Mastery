Let’s dive into **Day 8: Data Structures (Lists)**!  
Today, you’ll master **lists**, one of Python’s most versatile data structures, and learn to manipulate ordered collections of data. 📋  

---

### **Day 8: Data Structures (Lists)**  
**Objective**: Understand list operations, slicing, methods, and list comprehensions.  

---

#### **Step 1: What is a List?**  
- A **list** is an ordered, mutable collection of elements (can contain mixed data types).  
- Defined using square brackets `[]`.  

**Example**:  
```python  
fruits = ["apple", "banana", "cherry"]  
mixed_list = [10, "hello", 3.14, True]  
```  

---

#### **Step 2: List Operations**  
1. **Access Elements**:  
   ```python  
   print(fruits[0])   # Output: "apple" (index starts at 0)  
   print(fruits[-1])  # Output: "cherry" (negative index: -1 = last item)  
   ```  

2. **Modify Elements**:  
   ```python  
   fruits[1] = "blueberry"  # Replace "banana" with "blueberry"  
   ```  

3. **Check Length**:  
   ```python  
   print(len(fruits))  # Output: 3  
   ```  

---

#### **Step 3: List Methods**  
| Method      | Description                           | Example                            |  
|-------------|---------------------------------------|------------------------------------|  
| `append(x)` | Add `x` to the end                    | `fruits.append("orange")`          |  
| `insert(i, x)` | Insert `x` at index `i`           | `fruits.insert(1, "mango")`        |  
| `remove(x)` | Remove first occurrence of `x`        | `fruits.remove("apple")`           |  
| `pop(i)`    | Remove and return item at index `i`   | `popped = fruits.pop(2)`           |  
| `sort()`    | Sort the list (in-place)              | `numbers.sort()`                   |  
| `reverse()` | Reverse the list (in-place)           | `fruits.reverse()`                 |  

**Example**:  
```python  
numbers = [3, 1, 4, 1, 5]  
numbers.sort()  
print(numbers)  # Output: [1, 1, 3, 4, 5]  
```  

---

#### **Step 4: Slicing**  
Extract sublists using `list[start:end:step]`:  
- **start**: Inclusive (default = 0).  
- **end**: Exclusive (default = end of list).  
- **step**: Interval (default = 1).  

**Examples**:  
```python  
numbers = [0, 1, 2, 3, 4, 5]  
print(numbers[1:4])   # Output: [1, 2, 3] (indices 1 to 3)  
print(numbers[::2])   # Output: [0, 2, 4] (every 2nd element)  
print(numbers[::-1])  # Output: [5, 4, 3, 2, 1, 0] (reverse list)  
```  

---

#### **Step 5: List Comprehensions**  
Create lists concisely using a single line.  

**Syntax**:  
```python  
new_list = [expression for item in iterable if condition]  
```  

**Examples**:  
```python  
# Squares of numbers 0-9  
squares = [x**2 for x in range(10)]  

# Even numbers from a list  
evens = [x for x in numbers if x % 2 == 0]  
```  

---

#### **Step 6: Nested Lists**  
Lists can contain other lists (e.g., matrices):  
```python  
matrix = [  
    [1, 2, 3],  
    [4, 5, 6],  
    [7, 8, 9]  
]  
print(matrix[1][2])  # Output: 6 (2nd row, 3rd column)  
```  

---

### **Coding Exercises**  
1. **Basic List Manipulation**:  
   - Create a list of your top 3 hobbies.  
   - Add a new hobby, remove the second one, and print the final list.  

2. **Max/Min Finder**:  
   Write a function to find the maximum and minimum values in a list **without using `max()`/`min()`**.  

3. **List Comprehension Practice**:  
   Create a list of even numbers between 1 and 50 using a list comprehension.  

4. **Challenge (Flatten a Nested List)**:  
   Convert `[[1, 2], [3, [4, 5]], 6]` into `[1, 2, 3, 4, 5, 6]`.  
   *(Hint: Use recursion or loops!)*  

---

#### **Recap Questions**  
1. How do lists differ from strings in terms of mutability?  
2. What’s the output of `print([1, 2, 3][1:])`?  
3. Why are list comprehensions useful?  

---

#### **Common Mistakes**  
- Forgetting that list indices start at `0`.  
- Using `append()` instead of `extend()` to add multiple items.  
- Modifying a list while iterating over it (can cause errors).  

---

#### **What’s Next?**  
Tomorrow: **Day 9: Data Structures (Tuples & Sets)** – Immutable tuples and unique sets!  

---

**Your Task**:  
1. Share your solutions to the exercises.  
2. Try combining slicing and list methods (e.g., reverse a sublist).  

Let me know if you need help! 😊
