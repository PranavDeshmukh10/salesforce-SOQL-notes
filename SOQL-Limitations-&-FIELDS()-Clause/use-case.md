## ⚠️ SOQL Limitations & FIELDS() Clause  

> ❌ You **cannot** use `*` to select all fields in SOQL — unlike SQL!  

 As a workaround, use the `FIELDS()` clause, but note the **max LIMIT is 200 records**.  

## 🌐 Use Case 1 - Query all fields in contact object
 
## 💻 SOQL Query  
```soql
SELECT FIELDS(all) FROM Contact LIMIT 50 
```

## ✅ Hands-On Practice  
<img width="500" alt="35" src="https://github.com/user-attachments/assets/203e977d-c00a-4160-beff-2ac8940f339c" />

---
---

## 🌐 Use Case 2 - Query all standard fields of contact object
 
## 💻 SOQL Query  
```soql
SELECT FIELDS(standard) FROM Contact LIMIT 10
```

## ✅ Hands-On Practice  
<img width="500" alt="36" src="https://github.com/user-attachments/assets/52bad79a-78f0-47da-9814-4bad5bef87ec" />

---
---

## 🌐 Use Case 3 - Query all custom fields of contact object
 
## 💻 SOQL Query  
```soql
SELECT FIELDS(custom) FROM Contact LIMIT 10
```

## ✅ Hands-On Practice  
<img width="500" alt="37" src="https://github.com/user-attachments/assets/e0326118-a67f-44db-a107-28505392f44a" />

---
---

## 🌐 Use Case 4 - Query all custom fields and Id of opportunity object
 
## 💻 SOQL Query  
```soql
SELECT FIELDS(custom), Id FROM Contact LIMIT 10
```

## ✅ Hands-On Practice  
<img width="500" alt="38" src="https://github.com/user-attachments/assets/f4417a0d-cb8b-4c66-af24-08b0b9223948" />

<div align="center">

### 🚀 Happy Querying!

*Built with ❤️ for Salesforce Developers*

</div>
