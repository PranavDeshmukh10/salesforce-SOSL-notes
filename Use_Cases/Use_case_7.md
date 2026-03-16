## Use Case 7 — Find all contacts who have first name as Pranav but last name can be ‘Deshmukh’ or ‘Deshmukkh’

**Description:**
Find Contacts with first name `Pranav` but whose last name could be spelled as `Deshmukh` or `Deshmukkh` (common typo). The `IN` clause in the `WHERE` condition handles multiple possible values.

```sql
FIND {Pranav} IN NAME FIELDS RETURNING Contact(Id, FirstName, LastName WHERE FirstName = 'Pranav' AND LastName IN ('Deshmukh','Deshmukkh'))
```

📸 *Screenshot:*


*Happy Learning! 🚀*