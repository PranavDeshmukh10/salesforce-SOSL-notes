## Use Case 8 — Find the first 3 Account and Contact records with keyword ‘SMS’. Only filter those account which have revenue greater than 200K and contacts that have an email id. Record should be sorted based on Name.

**Description:**
Find top 3 Account and Contact records matching keyword `SMS`. Accounts must have annual revenue over 200K, Contacts must have an email. Results are sorted by Name. Demonstrates `ORDER BY`, `LIMIT`, and `WHERE` across multiple objects simultaneously.

```sql
FIND {SMS} IN ALL FIELDS RETURNING Account(Id, Name, AnnualRevenue WHERE AnnualRevenue > 200000 ORDER BY Name LIMIT 3), Contact(Id, Name, Email WHERE Email != null ORDER BY Name LIMIT 3)
```

📸 *Screenshot:*


*Happy Learning! 🚀*