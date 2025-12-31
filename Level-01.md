## Level 1 – Reading a File with a Special Name

### 🧩 Challenge
Locate and read a file that has a special character as its name in order to retrieve the password for the next level.

---

### 🔐 Access Details
Login name: bandit1  
Login password: Obtained from previous level  

---

### 🗂 What Was Available
After listing the directory, a file named `-` was present.  
Because the filename starts with a hyphen, it cannot be opened normally.

---

### ⚙️ Steps Performed
- ls  
- cat ./-  

---

### 📸 Proof of Work
![Level 1 Output](screenshots/level01.png)

---

### 🏁 Result
Password for the next level:  
263JGJPfgU6LtdEvfgWU1XP5yac29mFx

---

### 🧠 Why This Worked
Files that start with a hyphen are treated as command options.  
Using `./-` tells the shell that the hyphen is a filename in the current directory.

---

### 🛡️ Skill Gained
Understanding how Linux handles special characters in filenames and how to safely access them.
