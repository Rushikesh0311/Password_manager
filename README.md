# 🔐 Password Manager in C

This Password Manager securely stores and manages login credentials using XOR + HEX encryption. Data is protected with a Master Password, and credentials can be added, listed, searched, deleted, and edited.

## ⭐ Key Features
- Master Password authentication
- Add new credentials
- List credentials (auto-decrypted)
- Search credentials by site
- Delete specific credentials
- Reset master password
- Simple XOR + HEX encryption

## 📂 File Structure
```
│ main.c
│ comman.c
│ comman.h
│ credentials.csv      # Encrypted credentials stored here
│ meta.dat             # Master password stored here
│ README.md
```

## 🔐 How Encryption Works (Simple Explanation)

### 1) XOR Encryption
Each character in password is XORed with a key:
```
encrypted[i] = plain[i] ^ key;
```

### 2) Convert XOR Output to HEX
Because XOR result may be unprintable, we convert to HEX:
```
Byte -> Two Hex Characters
Example: 122 (z) -> 7A
```

### Example Conversion:
Password: `1234`

| Char | ASCII | XOR Key('K') | Result Char | HEX |
|-----|-------|--------------|-------------|-----|
| 1   | 49    | 75           | 122(z)      | 7A  |
| 2   | 50    | 75           | 121(y)      | 79  |
| 3   | 51    | 75           | 120(x)      | 78  |
| 4   | 52    | 75           | 127(DEL)    | 7F  |

Stored in file:  
```
7A79787F
```

During listing, HEX → XOR → original password restored ✅

---

## 🗃️ Example Stored in `credentials.csv`
```
3
github,rushi_dev,7A79787F
gmail,rushi.mail,6D7B7670
insta,rushi_0809,7F7A796C
```

## ✅ Decrypted Output (List View)
```
---------------------------------------------------------------
No   | Site         | Username        | Password
---------------------------------------------------------------
1    | github       | rushi_dev       | mypass123
2    | gmail        | rushi.mail      | mailpass09
3    | insta        | rushi_0809      | insta@098
---------------------------------------------------------------
```

---

## 🛠 Tools Used
- Language: C
- Compiler: GCC
- IDE: VS Code / Linux Terminal

## 🚀 Future Enhancements
| Feature | Status |
|--------|--------|
| AES Encryption | Coming Soon |
| GUI (GTK / Qt) | Planned |
| Password Strength Meter | Planned |
| Masked Password Input | Planned |

---

## 👨‍💻 Author
**Rushikesh Gore**  
GitHub: https://github.com/Rushikesh0311  
LinkedIn: https://www.linkedin.com/in/rushikeshgore11  
Email: **rushikeshgore0311@gmail.com**

---


