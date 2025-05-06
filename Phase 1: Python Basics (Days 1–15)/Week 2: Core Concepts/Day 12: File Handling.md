Let’s dive into **Day 12: File Handling**!  
Today, you’ll learn to read/write files, work with CSV/JSON data, and automate file operations. 📂  

---

### **Day 12: File Handling**  
**Objective**: Master file I/O operations and structured data formats (CSV/JSON).  

---

#### **Step 1: Reading Files**  
1. **Open a File**:  
   Use `open()` with modes:  
   - `"r"`: Read (default).  
   - `"w"`: Write (overwrites existing content).  
   - `"a"`: Append.  
   - `"r+"`: Read + write.  

   **Example**:  
   ```python  
   with open("data.txt", "r") as file:  
       content = file.read()  
   print(content)  
   ```  
   - `with` ensures the file closes automatically.  

2. **Read Line-by-Line**:  
   ```python  
   with open("data.txt") as file:  
       for line in file:  
           print(line.strip())  # Remove newline characters  
   ```  

---

#### **Step 2: Writing to Files**  
1. **Write to a New File**:  
   ```python  
   with open("output.txt", "w") as file:  
       file.write("Hello, World!\n")  
       file.write("Second line.")  
   ```  

2. **Append to an Existing File**:  
   ```python  
   with open("output.txt", "a") as file:  
       file.write("\nAppended text.")  
   ```  

---

#### **Step 3: Working with CSV Files**  
Use Python’s `csv` module for structured data.  

1. **Read CSV**:  
   ```python  
   import csv  
   with open("data.csv", "r") as file:  
       reader = csv.reader(file)  
       for row in reader:  
           print(row)  # Each row is a list  
   ```  

2. **Write CSV**:  
   ```python  
   data = [["Name", "Age"], ["Alice", 25], ["Bob", 30]]  
   with open("data.csv", "w") as file:  
       writer = csv.writer(file)  
       writer.writerows(data)  
   ```  

3. **Use `DictReader`/`DictWriter`** (for header-based CSV):  
   ```python  
   with open("data.csv", "r") as file:  
       reader = csv.DictReader(file)  
       for row in reader:  
           print(row["Name"], row["Age"])  
   ```  

---

#### **Step 4: Working with JSON Files**  
Use Python’s `json` module for JSON data.  

1. **Read JSON**:  
   ```python  
   import json  
   with open("data.json", "r") as file:  
       data = json.load(file)  # Returns a dictionary/list  
   print(data["key"])  
   ```  

2. **Write JSON**:  
   ```python  
   data = {"name": "Alice", "age": 25, "courses": ["Math", "Physics"]}  
   with open("data.json", "w") as file:  
       json.dump(data, file, indent=4)  # indent for pretty-print  
   ```  

---

### **Coding Exercises**  
1. **File Copier**:  
   Write a program to copy the contents of `source.txt` to `destination.txt`.  

2. **CSV Analyzer**:  
   Read a CSV file containing student grades and calculate the average grade.  

3. **JSON Config Parser**:  
   - Create a `config.json` file with settings like `{"language": "Python", "version": 3.12}`.  
   - Read it and print the values.  

4. **Challenge (CSV to JSON Converter)**:  
   Convert a CSV file to JSON format.  
   Example CSV:  
   ```csv  
   Name,Age  
   Alice,25  
   Bob,30  
   ```  
   Expected JSON:  
   ```json  
   [{"Name": "Alice", "Age": "25"}, {"Name": "Bob", "Age": "30"}]  
   ```  

---

#### **Recap Questions**  
1. What’s the difference between `"r"` and `"w"` modes?  
2. Why use `with open(...)` instead of `file = open(...)`?  
3. How does `json.load()` differ from `csv.reader()`?  

---

#### **Common Mistakes**  
- Forgetting to close files (always use `with`!).  
- Incorrect file paths (use absolute paths or check the working directory).  
- Mismatched headers in CSV `DictReader`/`DictWriter`.  

---

#### **What’s Next?**  
Tomorrow: **Day 13: Modules & Packages** – Organize code into reusable modules!  

---

**Your Task**:  
1. Complete the exercises and share your code.  
2. Try modifying the CSV analyzer to find the highest/lowest grade.  

Let me know if you need help! 😊
