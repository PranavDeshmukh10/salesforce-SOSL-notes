## Use Case 9 — Find all account records from My Accounts list view which have the keyword Acme.

**Description:**
Find Account records containing the keyword `Acme`, but only within the `My Accounts` list view. The `USING LISTVIEW` clause is helpful when you want to scope results to a specific saved view.

```sql
FIND {Account} IN ALL FIELDS RETURNING Account(Id, Name USING LISTVIEW = MyAccounts)
```

📸 *Screenshot:*


*Happy Learning! 🚀*