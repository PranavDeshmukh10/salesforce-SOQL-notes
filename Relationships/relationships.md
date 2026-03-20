<h1>🔗 Relationships</h1>

<h2>👇 Child to Parent (Query Parent Fields)</h2>

Use **dot notation** to traverse up to the parent record.

### 🌐 Query all Contacts with their parent Account Name where Billing City is San Francisco

### 💻 SOQL Query  
```soql
SELECT Name, AccountId, Account.Name, Account.BillingCity
FROM Contact
WHERE Account.BillingCity = 'San Francisco'
```

> 🔑 `Account.Name` = accessing a field on the **parent** Account from the **child** Contact.

### ✅ Hands-On Practice  
<img width="1000" alt="30" src="https://github.com/user-attachments/assets/32186cbf-76a0-4fbe-b3b0-a90d335f5a05" />

---
---

<h2>👇 Parent to Child (Query Child Fields)</h2>

Use a **inner query** with the child object's **relationship name** (usually plural).

### 🌐 Query all Accounts along with all their contacts where account SIC Code is 1452

### 💻 SOQL Query  
```soql
SELECT Id, Name, SIC, (SELECT Name FROM Contacts)
FROM Account
WHERE SIC = '1452'
```

> 🔑 `(SELECT Name FROM Contacts)` = fetching **child** Contact records from the **parent** Account.

### ✅ Hands-On Practice  
<img width="1000" height="864" alt="31" src="https://github.com/user-attachments/assets/a0267fe7-0643-44ac-beb8-3ae475c8382e" />


<div align="center">

### 🚀 Happy Querying!

*Built with ❤️ for Salesforce Developers*

</div>
