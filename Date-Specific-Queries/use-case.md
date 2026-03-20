## 📅 Use Case 1 - Find all cases which have been created in the current month

## 💻 SOQL Query  
```soql
SELECT Id, CaseNumber, Origin, CreatedDate FROM Case WHERE CreatedDate = THIS_MONTH
```

## ✅ Hands-On Practice  
<img width="500" alt="32" src="https://github.com/user-attachments/assets/4aa1c649-f77b-444e-9c45-d6463717f91d" />

---
---  

## 📅 Use Case 2 - Find all cases which have been created in the last month

## 💻 SOQL Query  
```soql
SELECT Id, CaseNumber, Origin, CreatedDate FROM Case WHERE CreatedDate = LAST_MONTH
```

## ✅ Hands-On Practice  
<img width="500" alt="33" src="https://github.com/user-attachments/assets/87386543-0360-4754-b91c-3bcbe88b90ce" />

---
---  

## 📅 Use Case 3 - Find all tasks which have been created between 7th Oct and 15th Nov

## 💻 SOQL Query  
```soql
SELECT Id, Subject, CreatedDate FROM Task WHERE CreatedDate >= 2025-10-07T00:00:00.000+0000 AND CreatedDate <= 2025-11-15T00:00:00.000+0000
```

## ✅ Hands-On Practice 
<img width="500" alt="34" src="https://github.com/user-attachments/assets/bb48b888-ef95-409f-bdfc-e775c7cbd98d" />
 
<div align="center">

### 🚀 Happy Querying!

*Built with ❤️ for Salesforce Developers*

</div>
