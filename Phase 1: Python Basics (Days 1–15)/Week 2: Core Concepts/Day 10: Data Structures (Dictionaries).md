Let’s dive into **Day 10: Data Structures (Dictionaries)**!  
Today, you’ll master **dictionaries** (key-value pairs), a cornerstone of Python for organizing and accessing data efficiently. 🗝️  

---

### **Day 10: Data Structures (Dictionaries)**  
**Objective**: Understand dictionaries, their methods, and use cases like data grouping and fast lookups.  

---

#### **Step 1: Basics of Dictionaries**  
- **Dictionary**: Unordered collection of `key: value` pairs.  
- Keys must be **unique** and **immutable** (strings, numbers, tuples).  
- Defined with curly braces `{}` or `dict()`.  

**Example**:  
```python  
student = {  
    "name": "Alice",  
    "age": 21,  
    "courses": ["Math", "Physics"]  
}  
```  

##### **Key Operations**:  
1. **Access Values**:  
   ```python  
   print(student["name"])      # Output: "Alice"  
   print(student.get("grade")) # Output: None (no KeyError)  
   ```  
2. **Modify/Add Entries**:  
   ```python  
   student["age"] = 22          # Update  
   student["grade"] = "A"       # Add new key  
   ```  
3. **Check Key Existence**:  
   ```python  
   if "courses" in student:  
       print("Courses exist!")  
   ```  

---

#### **Step 2: Dictionary Methods**  
| Method          | Description                          | Example                          |  
|-----------------|--------------------------------------|----------------------------------|  
| `keys()`        | Returns all keys                     | `student.keys()` → `dict_keys(["name", "age"])` |  
| `values()`      | Returns all values                   | `student.values()` → `dict_values(["Alice", 21])` |  
| `items()`       | Returns key-value pairs as tuples    | `student.items()` → `dict_items([("name", "Alice"), ...])` |  
| `get(key, default)` | Safely retrieve a value          | `student.get("grade", "N/A")` → `"N/A"` |  
| `update()`      | Merge dictionaries                   | `student.update({"grade": "A"})` |  
| `pop(key)`      | Remove a key and return its value    | `age = student.pop("age")` |  
| `popitem()`     | Remove and return last inserted item | `student.popitem()` → `("grade", "A")` |  

---

#### **Step 3: Dictionary Comprehensions**  
Create dictionaries concisely.  

**Syntax**:  
```python  
{key_expr: value_expr for item in iterable}  
```  

**Example**:  
```python  
squares = {x: x**2 for x in range(1, 6)}  
# Output: {1: 1, 2: 4, 3: 9, 4: 16, 5: 25}  
```  

---

#### **Step 4: Nested Dictionaries**  
Dictionaries can contain other dictionaries.  

**Example**:  
```python  
employees = {  
    "emp1": {"name": "Alice", "salary": 60000},  
    "emp2": {"name": "Bob", "salary": 75000}  
}  
print(employees["emp1"]["salary"])  # Output: 60000  
```  

---

### **Coding Exercises**  
1. **Basic Dictionary**:  
   - Create a dictionary for a book (title, author, year).  
   - Add a key `"genre"` and delete the year.  

2. **Invert Dictionary**:  
   Write a function to swap keys and values.  
   ```python  
   invert_dict({"a": 1, "b": 2}) → {1: "a", 2: "b"}  
   ```  

3. **Word Frequency Counter**:  
   Count how many times each word appears in a string.  
   ```python  
   text = "apple banana apple orange banana apple"  
   # Output: {"apple": 3, "banana": 2, "orange": 1}  
   ```  

4. **Challenge (Merge Dictionaries)**:  
   Merge two dictionaries. If keys overlap, keep the value from the second dict.  
   ```python  
   dict1 = {"a": 1, "b": 2}  
   dict2 = {"b": 3, "c": 4}  
   # Output: {"a": 1, "b": 3, "c": 4}  
   ```  

5. **Nested Dictionary Practice**:  
   Create a nested dictionary for 3 employees with name, role, and salary.  
   Calculate the average salary.  

---

#### **Recap Questions**  
1. Why can’t a list be a dictionary key?  
2. What’s the difference between `dict["key"]` and `dict.get("key")`?  
3. How does `items()` differ from `keys()`?  

---

#### **Common Mistakes**  
- Using mutable types (e.g., lists) as keys.  
- Assuming dictionaries preserve insertion order (true in Python 3.7+ but not guaranteed earlier).  
- Misspelling keys (case-sensitive!).  

---

#### **What’s Next?**  
Tomorrow: **Day 11: Error Handling** – Learn to handle exceptions with `try-except`!  

---

**Your Task**:  
1. Share your code for the exercises.  
2. Experiment with nested dictionaries (e.g., student → courses → grades).  

Let me know if you need help debugging! 😊
