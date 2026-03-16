## 🧩 Use Case — Find all contacts who have first name as Pranav but last name can be ‘Deshmukh’ or ‘Deshmukkh’

**Description:**
Find Contacts with first name `Pranav` but whose last name could be spelled as `Deshmukh` or `Deshmukkh` (common typo). The `IN` clause in the `WHERE` condition handles multiple possible values.

## 🛠️ Solution  
```sql
FIND {Pranav} IN NAME FIELDS RETURNING Contact(Id, FirstName, LastName WHERE FirstName = 'Pranav' AND LastName IN ('Deshmukh','Deshmukkh'))
```

## ✅ Hands On Practice   
<img width="1000" alt="8" src="https://github.com/user-attachments/assets/830043ed-05e7-48b5-bd20-f25f0b47af2b" />  

*Happy Learning! 🚀*
