## Level 29 – Finding Hidden Credentials in a Different Git Branch

### 🧩 Challenge
The password is not present in the main branch.  
Switch to another Git branch to locate the hidden credentials.

---

### 🔐 Access Details
Login name: bandit29  
Login password: Obtained from previous level  

---

### 🗂 What Was Available
The repository contained multiple branches, including `dev`.  
The main branch showed a placeholder instead of the real password.

---

### ⚙️ Steps Performed
- git clone ssh://bandit29-git@bandit.labs.overthewire.org:2220/home/bandit29-git/repo  
- cd repo  
- git branch -a  
- git checkout dev  
- git log -p  

---

### 📸 Proof of Work

**Switching to the dev branch and viewing the commit history**  
![Branch switch](Screenshots/level29_1.png)

-

**Finding the password inside the README diff**  
![Password found](Screenshots/level29_2.png)

---

### 🏁 Result
Password for the next level:  
qp30ex3VLz5MDG1n91YowTv4Q81CDZL

---

### 🧠 Why This Worked
The `dev` branch contained development data that was not merged into `master`.  
By inspecting its commit history, the real password was revealed.

---

### 🛡️ Skill Gained
Understanding how to explore multiple Git branches to uncover hidden or unreleased information.
