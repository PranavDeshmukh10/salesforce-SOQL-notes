<h1>🚫 Using NULL in Queries</h1>

**Example:**
```sql
SELECT Id, Name, NumberOfEmployees
FROM Account
WHERE NumberOfEmployees != null
```
---

<h2> 👥 Use Case 1 - Find all Accounts where Number of Employees are not Null</h2>

### 💻 SOQL Query  
```soql
SELECT Id, Name, NumberOfEmployees FROM Account WHERE NumberOfEmployees != null
```

### ✅ Hands-On Practice  
<img width="700" alt="24" src="https://github.com/user-attachments/assets/06bdc676-f696-43b6-96c8-92f9840fa9fe" />

---
---

<h2> 🔗 Use Case 2 - Find all Contacts where Parent Account doesn’t exist</h2>

### 💻 SOQL Query  
```soql
SELECT Id, Name, AccountId FROM Contact WHERE AccountId = null
```

### ✅ Hands-On Practice  
<img width="700" alt="25" src="https://github.com/user-attachments/assets/d392791a-9149-456a-925a-185152ca1823" />

---
---

<h2> 📭 Use Case 3 - Find all Cases where Case Origin is not specified.</h2>

### 💻 SOQL Query  
```soql
SELECT Id, CaseNumber, Origin FROM Case WHERE Origin = null
```

### ✅ Hands-On Practice  
<img width="700" alt="26" src="https://github.com/user-attachments/assets/206e15c4-a756-49e1-a2e6-61d27871c28c" />

---
---

<h2> 🌐 Use Case 4 - Find all Leads where Lead Source is specified.</h2>

### 💻 SOQL Query  
```soql
SELECT Id, Name, LeadSource FROM Lead WHERE LeadSource != null
```

### ✅ Hands-On Practice  
<img width="700" alt="27" src="https://github.com/user-attachments/assets/0d680124-9b52-4a4f-a082-ea80aa17f1ce" />


<div align="center">

### 🚀 Happy Querying!

*Built with ❤️ for Salesforce Developers*

</div>
