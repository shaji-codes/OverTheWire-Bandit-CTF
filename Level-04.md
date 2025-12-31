## Level 4 – Identifying the Correct Data File

### 🧩 Challenge
Inside a directory containing many files, identify the one file that contains readable text and extract the password.

---

### 🔐 Access Details
Login name: bandit4  
Login password: Obtained from previous level  

---

### 🗂 What Was Available
The `inhere` directory contained many files with similar names. Most of them were binary data, and only one contained readable ASCII text.

---

### ⚙️ Steps Performed
- ls  
- cd inhere  
- ls -alph  
- find . -type f | xargs file  
- cat ./-file07  

---

### 📸 Proof of Work
![Level 4 Output](Screenshots/level04.png)

---

### 🏁 Result
Password for the next level:  
4oQYVPkxZOOEOtSkbE8j8p8YXGUQw

---

### 🧠 Why This Worked
The `file` command identifies the type of data inside each file.  
By checking all files, the one labeled as **ASCII text** was selected and read to reveal the password.

---

### 🛡️ Skill Gained
Learning how to inspect unknown files and identify which
