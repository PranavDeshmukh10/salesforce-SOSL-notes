## 🧩  Use Case — Find all Leads with name which is either “David” or “Betty” and only show records which have been modified today 

**Description:**
Find Lead records where the name is either `David` or `Betty`, and only return records that were modified today. Demonstrates use of `OR` keyword and `WHERE` with date filters.

## 🛠️ Solution  
```sql
FIND {David OR Betty} IN NAME FIELDS RETURNING Lead(Id, Name, CreatedDate, LastModifiedDate WHERE LastModifiedDate = Today)
```

## ✅ Hands On Practice   
<img width="1000" alt="5" src="https://github.com/user-attachments/assets/d210c896-dbd7-4b57-a503-ac55fe427546" />


*Happy Learning! 🚀*
