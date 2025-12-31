## Level 0 – Getting Inside the Bandit Server

### 🧩 Challenge
Connect to the Bandit game server for the first time and locate the password required to enter the next level.

---

### 🔐 Access Details
Login name: bandit0  
Login password: bandit0  

---

### 🗂 What Was Available
After logging in, a file named `readme` was found in the home directory.  
This file contained instructions and the password for the next level.

---

### ⚙️ Steps Performed
- ls  
- cat readme  

---

### 📸 Proof of Work

![Level 0 Output](Screenshots/level00.png)

---

### 🏁 Result
Password for the next level:  
ZJljTmM6FvvyRnrb2rfNWOZOTa6ip5If

---

### 🧠 Why This Worked
The server stores important information inside plain text files. By listing files and reading their contents, hidden credentials can be revealed.

---

### 🛡️ Skill Gained
Learning how to navigate a Linux directory and read files to extract sensitive data.
