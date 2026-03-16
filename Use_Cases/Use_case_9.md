## 🧩 Use Case — Find all account records from My Accounts list view which have the keyword Acme.

**Description:**
Find Account records containing the keyword `Acme`, but only within the `My Accounts` list view. The `USING LISTVIEW` clause is helpful when you want to scope results to a specific saved view.

## 🛠️ Solution  
```sql
FIND {Account} IN ALL FIELDS RETURNING Account(Id, Name USING LISTVIEW = MyAccounts)
```

## ✅ Hands On Practice   
<img width="1000" alt="11" src="https://github.com/user-attachments/assets/d2875782-e6f0-4c4f-bdee-740ec128498b" />


*Happy Learning! 🚀*
