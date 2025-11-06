# Password_manager
<!-- Stylish Header -->
<h1 align="center">🔐 Password Manager in C</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Language-C-blue.svg" alt="Language"/>
  <img src="https://img.shields.io/badge/Concept-File Handling-yellow.svg" alt="File Handling"/>
  <img src="https://img.shields.io/badge/Topic-Data Encryption & Management-orange.svg" alt="Data Management"/>
  <img src="https://img.shields.io/badge/IDE-VS Code-lightgrey.svg" alt="IDE"/>
</p>

<p align="center">
  <b>Developed by <a href="https://github.com/Rushikesh0311">Rushikesh Gore</a></b>  
</p>

---

## 🧩 Overview
The **Password Manager in C** is a secure and simple command-line application that helps users **store, view, search, and manage passwords** for multiple accounts.  
It uses **file handling** to maintain encrypted credentials locally and includes a **master password** feature to protect all saved data.

---

## 📘 Project Description
This project demonstrates the use of **file handling, string operations, and modular functions in C**.  
It simulates a password vault where each credential (website, username, password) is securely stored and can only be accessed after master authentication.

🔹 **Master Password:** Protects all credentials  
🔹 **Add Credential:** Save a new website login securely  
🔹 **View Credential:** List stored passwords (decrypted)  
🔹 **Search Credential:** Find specific website login details  
🔹 **Reset Master Password:** Securely update your vault access  

---

## 🌟 Features
✅ Master password-based access control  
✅ Add, list, and search saved credentials  
✅ Passwords stored in encrypted (hex) format  
✅ Option to reset master password  
✅ Modular code with separate `.c` and `.h` files  
✅ File-based permanent storage  
✅ Simple menu-driven interface  

---

## 📂 File Structure
```
Password_Manager/
│
├── main.c               # Entry point and main menu
├── comman.c             # Core functions (add, list, search, encryption, etc.)
├── comman.h             # Function declarations and structures
├── credentials.dat      # Encrypted credentials storage
├── master.dat           # Master password storage
├── README.md            # Project documentation
```

---

## 🧠 Core Functions
| Function | Description |
|-----------|--------------|
| `add_credentials()` | Adds new login info |
| `list_credentials()` | Displays all saved accounts |
| `search_credentials()` | Searches for a specific account |
| `verify_master_pass()` | Authenticates master password |
| `reset_master_pass()` | Allows resetting master password |
| `text_to_hex()` | Encrypts text for safe storage |
| `hex_to_text()` | Decrypts text for display |

---

## ⚙️ Build and Run
### ▶️ Compile the Program
```bash
gcc *.c -o password_manager
```

### ▶️ Run the Program
```bash
./password_manager
```

---

## 🖥️ Sample Outputs

### 🔑 **1. Master Password Verification**
```bash
-----------------------------------
Welcome to Password Manager
-----------------------------------
Enter Master Password: ******
✅ Access Granted!
```

---

### 🆕 **2. Add a New Credential**
```bash
========= ADD NEW CREDENTIAL =========
Enter Website : github.com
Enter Username: rushikesh
Enter Password: mySecure@123
--------------------------------------
✅ Credential Saved Successfully!
```

---

### 📋 **3. View All Saved Credentials**
```bash
========= STORED CREDENTIALS =========
Website : github.com
Username: rushikesh
Password: mySecure@123
--------------------------------------
Website : gmail.com
Username: rushi0311
Password: password@321
======================================
```

---

### 🔍 **4. Search a Credential**
```bash
========= SEARCH CREDENTIAL =========
Enter Website to search: github.com

Website : github.com
Username: rushikesh
Password: mySecure@123
--------------------------------------
✅ Match Found!
```

---

### 🔄 **5. Reset Master Password**
```bash
========= RESET MASTER PASSWORD =========
Enter Old Master Password: ******
✅ Verified Successfully!

Enter New Master Password: ********
Confirm Password: ********
✅ Master Password Reset Successfully!
Returning to Main Menu...
```

---

## 💡 Ideal For
- Students learning **File Handling in C**
- Mini projects for **College or Internship Submissions**
- Understanding **Data Security and Encryption Basics**
- Practicing **Menu-driven and Modular C Programs**

---

## 🧰 Tools & Environment
- **Language:** C  
- **Compiler:** GCC  
- **IDE Used:** VS Code / Code::Blocks  
- **OS Tested On:** Linux / Windows  

---

## 🚀 Future Enhancements
- 🔒 Implement stronger encryption (e.g., AES)  
- 🧮 Add password strength analyzer  
- ☁️ Cloud sync for credentials  
- 📱 Create a GUI version (using GTK or C++)  
- 🧾 Add option to export credentials to CSV  

---

## 👨‍💻 Author
**Rushikesh Gore**  
📧 Email: [rushikeshgore0311@gmail.com](mailto:rushikeshgore0311@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/rushikeshgore11) | [GitHub](https://github.com/Rushikesh0311)

---
