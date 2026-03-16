## 🧩 Use Case — Find all contacts where Name is Pranav showing the name and phone information

**Description:**
Find all Contacts named `Pranav` and return only specific fields — `Id`, `FirstName`, `LastName`, and `Phone`. Useful when you don't need the full record.

## 🛠️ Solution  
```sql
FIND {Pranav} IN Name FIELDS RETURNING Contact(Id, FirstName, LastName, Phone)
```

## ✅ Hands On Practice   
<img width="1000" alt="4" src="https://github.com/user-attachments/assets/5ac8bff8-fda9-402e-b920-6795eca0cfdf" />


*Happy Learning! 🚀*
