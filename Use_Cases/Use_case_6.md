## Use Case 6 — Find all Web Sourced contact &  Active user records where name is Pranav

**Description:**
Find both Contact and User records named `Pranav`, but apply different filters to each — only Web-sourced Contacts and only Active Users. Shows how SOSL can query multiple objects in a single call.

```sql
FIND {Pranav} IN NAME FIELDS RETURNING Contact(Id, Name, LeadSource WHERE LeadSource = 'Web'), User(Id, Name, IsActive WHERE IsActive = true)
```

📸 *Screenshot:*


*Happy Learning! 🚀*