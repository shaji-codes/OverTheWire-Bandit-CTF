## Level 27 – Retrieving a Password from a Git Repository

### 🧩 Challenge
Clone a remote Git repository hosted on the Bandit server and locate the password for the next level inside it.

---

### 🔐 Access Details
Login name: bandit27  
Login password: Obtained from previous level  

---

### 🗂 What Was Available
A Git repository was hosted at:  
`ssh://bandit27-git@bandit.labs.overthewire.org:2220/home/bandit27-git/repo`  

This repository contained a README file that stored the password for the next level.

---

### ⚙️ Steps Performed
- git clone ssh://bandit27-git@bandit.labs.overthewire.org:2220/home/bandit27-git/repo  
- cd repo  
- cat README  

---

### 📸 Proof of Work

**Cloning the repository and reading the README file**  
![Git clone and read](Screenshots/level27.png)

---

### 🏁 Result
Password for the next level:  
Yz9lpLoSBcCeuG7m9uQFt8zNpS4HZRcN

---

### 🧠 Why This Worked
The password was stored in plain text inside the Git repository.  
By cloning it over SSH and reading the README file, the password could be retrieved.

---

### 🛡️ Skill Gained
Understanding how to access and analyze remote Git repositories over SSH to extract stored information.
