## 🧩 Use Case — Find all Web Sourced contact &  Active user records where name is Pranav

**Description:**
Find both Contact and User records named `Pranav`, but apply different filters to each — only Web-sourced Contacts and only Active Users. Shows how SOSL can query multiple objects in a single call.

## 🛠️ Solution  

```sql
FIND {Pranav} IN NAME FIELDS RETURNING Contact(Id, Name, LeadSource WHERE LeadSource = 'Web'), User(Id, Name, IsActive WHERE IsActive = true)
```

## ✅ Hands On Practice   
<img width="1000" alt="6" src="https://github.com/user-attachments/assets/251c5637-9962-4940-bb26-dda82c6b85d7" />  
<img width="1000" alt="7" src="https://github.com/user-attachments/assets/79ade00c-2f72-46c5-acc6-1e22c8d0e54f" />  


*Happy Learning! 🚀*
