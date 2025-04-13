Let’s dive into **Day 9: Data Structures (Tuples & Sets)**!  
Today, you’ll explore **tuples** (immutable sequences) and **sets** (unordered unique collections). 🧩  

---

### **Day 9: Data Structures (Tuples & Sets)**  
**Objective**: Master tuples and sets, their properties, and use cases.  

---

#### **Step 1: Tuples**  
- **Tuples** are **immutable** (cannot be modified after creation).  
- Defined with parentheses `()` or commas.  
- Ideal for fixed data (e.g., coordinates, database records).  

**Example**:  
```python  
coordinates = (3, 5)  
colors = "red", "green", "blue"  # Parentheses optional  
```  

##### **Key Operations**:  
1. **Access Elements**:  
   ```python  
   print(coordinates[0])  # Output: 3  
   ```  
2. **Slicing**: Same as lists (`tuple[start:end]`).  
3. **Methods**:  
   - `count(x)`: Returns the number of occurrences of `x`.  
   - `index(x)`: Returns the first index of `x`.  

**Immutability Example**:  
```python  
coordinates[0] = 10  # Error: Tuples are immutable!  
```  

---

#### **Step 2: Sets**  
- **Sets** store **unique**, **unordered** elements.  
- Defined with curly braces `{}` or `set()`.  
- Used for membership testing, removing duplicates, and mathematical operations.  

**Example**:  
```python  
fruits = {"apple", "banana", "cherry"}  
unique_numbers = set([1, 2, 2, 3])  # Output: {1, 2, 3}  
```  

##### **Key Operations**:  
| Method/Operator | Description                     | Example                          |  
|-----------------|---------------------------------|----------------------------------|  
| `add(x)`        | Add element `x`                 | `fruits.add("orange")`           |  
| `remove(x)`     | Remove `x` (error if missing)   | `fruits.remove("apple")`         |  
| `discard(x)`    | Remove `x` (no error)           | `fruits.discard("mango")`        |  
| `union()`       | Combine sets (`|`)              | `set1 | set2`                      |  
| `intersection()`| Common elements (`&`)           | `set1 & set2`                    |  
| `difference()`  | Elements in `set1` not in `set2` (`-`)| `set1 - set2`              |  

**Example**:  
```python  
A = {1, 2, 3}  
B = {3, 4, 5}  
print(A | B)  # Output: {1, 2, 3, 4, 5}  
```  

##### **Frozen Sets**:  
- Immutable version of sets: `frozenset()`.  
- Cannot add/remove elements.  

---

### **Coding Exercises**  
1. **Tuple Practice**:  
   - Create a tuple of your favorite movies.  
   - Try to modify it (observe the error) and convert it to a list.  

2. **Set Operations**:  
   - Remove duplicates from `[1, 2, 2, 3, 4, 4, 5]` using a set.  
   - Check if two lists have common elements:  
     ```python  
     list1 = [1, 2, 3]  
     list2 = [3, 4, 5]  
     common = set(list1) & set(list2)  
     ```  

3. **Challenge (Vowel Counter)**:  
   Use a set to count the number of unique vowels in a string.  
   ```python  
   text = "Hello, World!"  
   vowels = {"a", "e", "i", "o", "u"}  
   unique_vowels = set(text.lower()) & vowels  
   print(len(unique_vowels))  # Output: 3 (e, o, o is counted once)  
   ```  

4. **Tuple Unpacking**:  
   Unpack coordinates `(x, y, z) = (5, 10, 15)` and print each value.  

---

#### **Recap Questions**  
1. Why can’t you use a list as a set element?  
2. How do tuples differ from sets in terms of order and mutability?  
3. What’s the result of `set([1, 1, 2, 3])`?  

---

#### **Common Mistakes**  
- Trying to modify a tuple (immutable).  
- Assuming sets preserve order (they don’t!).  
- Using `{}` for an empty set (it creates a dict; use `set()`).  

---

#### **What’s Next?**  
Tomorrow: **Day 10: Data Structures (Dictionaries)** – Key-value pairs and advanced methods!  

---

**Your Task**:  
1. Share your code for the exercises.  
2. Try creating a set of tuples (e.g., `{(1, 2), (3, 4)}`).  

Let me know if you get stuck! 😊
