Let’s dive into **Day 13: Modules & Packages**!  
Today, you’ll learn to organize code into reusable modules, import them, and create your own packages. 📦  

---

### **Day 13: Modules & Packages**  
**Objective**: Understand Python modules, packages, and how to structure code for reusability.  

---

#### **Step 1: What is a Module?**  
- A **module** is a Python file (`.py`) containing functions, classes, or variables.  
- You can import modules to reuse code across files.  

**Example**:  
Create a file `math_utils.py`:  
```python  
# math_utils.py  
def add(a, b):  
    return a + b  

def multiply(a, b):  
    return a * b  
```  

In another file:  
```python  
# main.py  
import math_utils  

result = math_utils.add(2, 3)  
print(result)  # Output: 5  
```  

---

#### **Step 2: Importing Modules**  
1. **Import Entire Module**:  
   ```python  
   import math_utils  
   ```  

2. **Import Specific Functions**:  
   ```python  
   from math_utils import add, multiply  
   print(add(2, 3))  
   ```  

3. **Import with Alias**:  
   ```python  
   import math_utils as mu  
   print(mu.multiply(2, 3))  
   ```  

4. **Import All Functions** (not recommended):  
   ```python  
   from math_utils import *  
   ```  

---

#### **Step 3: Standard Library Modules**  
Python comes with built-in modules. Examples:  
- `math`: Mathematical functions.  
- `random`: Generate random numbers.  
- `datetime`: Work with dates and times.  

**Example**:  
```python  
import math  
print(math.sqrt(25))  # Output: 5.0  

import random  
print(random.randint(1, 10))  # Random integer between 1 and 10  

from datetime import datetime  
print(datetime.now())  # Current date and time  
```  

---

#### **Step 4: What is a Package?**  
- A **package** is a directory containing multiple modules (and a special `__init__.py` file).  
- Used to organize related modules.  

**Example Structure**:  
```
my_package/  
    __init__.py  
    math_utils.py  
    string_utils.py  
```  

- `__init__.py` can be empty or initialize the package.  

**Import from a Package**:  
```python  
from my_package import math_utils  
from my_package.string_utils import reverse_string  
```  

---

#### **Step 5: Creating Your Own Package**  
1. Create a directory: `my_package`.  
2. Add `__init__.py` (can be empty).  
3. Add modules (e.g., `math_utils.py`).  

**Example `__init__.py`**:  
```python  
# Import key functions for easier access  
from .math_utils import add, multiply  
from .string_utils import reverse_string  
```  

Now you can use:  
```python  
import my_package  
print(my_package.add(2, 3))  
```  

---

#### **Step 6: The `if __name__ == "__main__"` Guard**  
- Allows code to run only when the script is executed directly (not when imported).  

**Example**:  
```python  
# math_utils.py  
def add(a, b):  
    return a + b  

if __name__ == "__main__":  
    # Test code  
    print(add(5, 10))  # Runs only if executed directly  
```  

---

### **Coding Exercises**  
1. **Create a Module**:  
   - Create a module `greetings.py` with a function `greet(name)` that returns a greeting.  
   - Import and use it in `main.py`.  

2. **Use the `math` Module**:  
   - Calculate the area of a circle using `math.pi`.  

3. **Build a Package**:  
   - Create a package `utils` with two modules:  
     - `math_utils.py` (with `add`, `multiply`).  
     - `string_utils.py` (with `reverse_string`, `capitalize`).  
   - Import and use them in a script.  

4. **Challenge (Random Password Generator)**:  
   Use the `random` module to generate a random password of length 8 (with letters and digits).  

---

#### **Recap Questions**  
1. What is the purpose of `__init__.py`?  
2. How do you import a function from a module in a package?  
3. Why use `if __name__ == "__main__"`?  

---

#### **Common Mistakes**  
- Forgetting to include `__init__.py` in a package.  
- Naming modules after built-in modules (e.g., `math.py`).  
- Circular imports (module A imports module B, and vice versa).  

---

#### **What’s Next?**  
Tomorrow: **Day 14: Recap & Exercises** – Reinforce modules and packages with practice!  

---

**Your Task**:  
1. Build the `greetings` module and share your code.  
2. Create the `utils` package and test its functions.  

Let me know if you get stuck! 😊
