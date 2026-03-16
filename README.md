
# <img width="110" alt="SOSL_Logo" src="https://github.com/user-attachments/assets/96a01d27-170a-46d5-8e4a-e54724efe3f9" /> 🔍 SALESFORCE OBJECT SEARCH LANGUAGE (SOSL)

> A practical guide to SOSL (Salesforce Object Search Language) — covering syntax, real-world use cases, filters, multi-object search, governor limits and more.

---

## 📌 What is SOSL?

**SOSL (Salesforce Object Search Language)** is a search language used to perform text-based searches across multiple Salesforce objects and fields simultaneously. Unlike SOQL (which queries a single object), SOSL can search across multiple objects in a single query — making it ideal for global search scenarios.

### SOSL vs SOQL — Quick Comparison

| Feature | SOSL | SOQL |
|---|---|---|
| Search across | Multiple objects | Single object |
| Search type | Text/keyword search | Structured query |
| Use case | Global search | Precise data retrieval |
| Keyword | `FIND` | `SELECT` |

---

## 🧱 Basic SOSL Syntax

```sql
FIND {SearchQuery}
  [IN SearchGroup]
  [RETURNING ObjectsAndFields]
  [WHERE FilterCondition]
  [ORDER BY Field]
  [LIMIT n]
```

---

## 🔑 Key Clauses Reference

| Clause | Purpose | Example |
|---|---|---|
| `FIND {}` | Search keyword | `FIND {Pranav}` |
| `IN ... FIELDS` | Scope of search | `IN Name FIELDS`, `IN ALL FIELDS`, `IN Email FIELDS` |
| `RETURNING` | Which objects/fields to return | `RETURNING Contact(Id, Name)` |
| `WHERE` | Filter records | `WHERE IsActive = true` |
| `ORDER BY` | Sort results | `ORDER BY Name` |
| `LIMIT` | Cap number of results | `LIMIT 3` |
| `USING LISTVIEW` | Search within a list view | `USING LISTVIEW = MyAccounts` |

---

## ⚠️ Governor Limits

Salesforce enforces the following limits for SOSL:

| Limit | Value |
|---|---|
| Max SOSL queries per transaction | **20** |
| Max records returned per query | **2,000** |

> 💡 Always keep governor limits in mind when designing automation or Apex code that uses SOSL.

---

## 📂 Repo Structure

```
📦 your-repo
 ┣ 📄 README.md
 ┗ 📄 USE_CASES.md
```

- **README.md** — Overview, syntax, key clauses & governor limits
- **USE_CASES.md** — 9 hands-on SOSL queries with descriptions & screenshots

---

## 📚 Resources

- [Salesforce SOSL Official Documentation](https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm)
- [Trailhead — SOSL Module](https://trailhead.salesforce.com/content/learn/modules/apex_database/apex_database_sosl)

---

## 🙋 About

This repo documents my hands-on SOSL learning journey as part of my Salesforce development path.
Feel free to fork, star ⭐, or use this as a reference in your own Trailblazer journey!

---

*Happy Learning! 🚀*
