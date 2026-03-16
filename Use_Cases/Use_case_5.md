## Use Case 5 — Find all Leads with name which is either “David” or “Betty” and only show records which have been modified today 

**Description:**
Find Lead records where the name is either `David` or `Betty`, and only return records that were modified today. Demonstrates use of `OR` keyword and `WHERE` with date filters.

```sql
FIND {David OR Betty} IN NAME FIELDS RETURNING Lead(Id, Name, CreatedDate, LastModifiedDate WHERE LastModifiedDate = Today)
```

📸 *Screenshot:*


*Happy Learning! 🚀*