## Level 25 – Logging in Using an SSH Private Key

### 🧩 Challenge
Use the provided SSH private key from the current level to log in as the next user and obtain the password.

---

### 🔐 Access Details
Login name: bandit25  
Login password: Obtained from previous level  

---

### 🗂 What Was Available
A file named `bandit26.sshkey` was available in the home directory of `bandit25`.  
This private key allows SSH access to the `bandit26` account.

---

### ⚙️ Steps Performed
- scp -P 2220 bandit25@bandit.labs.overthewire.org:/home/bandit25/bandit26.sshkey .  
- chmod 600 bandit26.sshkey  
- ssh -i bandit26.sshkey bandit26@bandit.labs.overthewire.org -p 2220  

---

### 📸 Proof of Work

**Copying the SSH private key from the Bandit server**  
![SSH key copy](Screenshots/level25_2.png)

-

**Using the private key to log in as bandit26**  
![SSH login](Screenshots/level25_3.png)

-

**Successful login into bandit26**  
![Login success](Screenshots/level25_5.png)

---

### 🏁 Result
Password for the next level:  
s07zxWkK0MxfqO0FPRv9L3jJBU0GZ

---

### 🧠 Why This Worked
SSH supports key-based authentication.  
By copying the private key, setting proper permissions, and using it with SSH, access to `bandit26` was granted.

---

### 🛡️ Skill Gained
Understanding how SSH private keys can be used to authenticate users securely without passwords.
