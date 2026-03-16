## 🧩 Use Case — Find all contact records whose email is abc@gmail.com

**Description:**
Search for Contact records where the email matches `abc@gmail.com`. The `RETURNING Contact` clause ensures only Contact object results are returned.

## 🛠️ Solution
```sql
FIND {abc@gmail.com} IN Email FIELDS RETURNING Contact
```

## ✅ Hands On Practice   
<img width="1000" alt="3" src="https://github.com/user-attachments/assets/b3a41063-8119-41cf-8814-c3338e9878da" />


*Happy Learning! 🚀*
