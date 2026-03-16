## Use Case 3 — Find all contact records whose email is abc@gmail.com

**Description:**
Search for Contact records where the email matches `abc@gmail.com`. The `RETURNING Contact` clause ensures only Contact object results are returned.

```sql
FIND {abc@gmail.com} IN Email FIELDS RETURNING Contact
```

📸 *Screenshot:*


*Happy Learning! 🚀*