## Use Case 4 — Find all contacts where Name is Pranav showing the name and phone information

**Description:**
Find all Contacts named `Pranav` and return only specific fields — `Id`, `FirstName`, `LastName`, and `Phone`. Useful when you don't need the full record.

```sql
FIND {Pranav} IN Name FIELDS RETURNING Contact(Id, FirstName, LastName, Phone)
```

📸 *Screenshot:*


*Happy Learning! 🚀*