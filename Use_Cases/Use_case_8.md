## 🧩 Use Case — Find the first 3 Account and Contact records with keyword ‘SMS’. Only filter those account which have revenue greater than 200K and contacts that have an email id. Record should be sorted based on Name.

**Description:**
Find top 3 Account and Contact records matching keyword `SMS`. Accounts must have annual revenue over 200K, Contacts must have an email. Results are sorted by Name. Demonstrates `ORDER BY`, `LIMIT`, and `WHERE` across multiple objects simultaneously.

## 🛠️ Solution  
```sql
FIND {SMS} IN ALL FIELDS RETURNING Account(Id, Name, AnnualRevenue WHERE AnnualRevenue > 200000 ORDER BY Name LIMIT 3), Contact(Id, Name, Email WHERE Email != null ORDER BY Name LIMIT 3)
```

## ✅ Hands On Practice   
<img width="1000" alt="9" src="https://github.com/user-attachments/assets/cceca80f-6085-464e-b5bc-c1bed4a2bb48" />  
<img width="1000" alt="10" src="https://github.com/user-attachments/assets/f8c22984-d8ae-4f9d-a650-7635156efc2a" />  


*Happy Learning! 🚀*
