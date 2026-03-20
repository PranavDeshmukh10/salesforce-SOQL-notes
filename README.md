# <img width="110" alt="ChatGPT Image Mar 20, 2026, 07_00_16 AM" src="https://github.com/user-attachments/assets/9cc17f93-12f4-4ce6-820a-84fa86095907" /> 📘 SALESFORCE OBJECT QUERY LANGUAGE (SOQL)

> 🌟 A comprehensive reference guide for SOQL with practical use cases, operators, relationships, and examples.

<div align="center">

![Salesforce](https://img.shields.io/badge/Salesforce-00A1E0?style=for-the-badge&logo=salesforce&logoColor=white)
![SOQL](https://img.shields.io/badge/SOQL-Query%20Language-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

</div>

---

## 📚 Table of Contents

| # | Topic |
|---|---|
| 1 | [🤔 What is SOQL?](#-what-is-soql) |
| 2 | [❓ Why do we need SOQL?](#-why-do-we-need-soql) |
| 3 | [🏗️ Query Structure](#%EF%B8%8F-query-structure) |
| 4 | [🔍 Querying Fields](#-querying-fields) |
| 5 | [✅ Use Cases with WHERE Clause](#-use-cases-with-where-clause) |
| 6 | [⚙️ Operators](#%EF%B8%8F-operators) |
| 7 | [🚫 Using NULL in Queries](#-using-null-in-queries) |
| 8 | [✔️ Using Boolean Flags](#%EF%B8%8F-using-boolean-flags) |
| 9 | [🔗 Relationships](#-relationships) |
| 10 | [📅 Date Specific Queries](#-date-specific-queries) |
| 11 | [🔒 Escape & Reserved Characters](#-escape--reserved-characters) |
| 12 | [⚠️ SOQL Limitations & FIELDS() Clause](#%EF%B8%8F-soql-limitations--fields-clause) |
| 13 | [📏 Governor Limits](#-governor-limits) |

---

## 🤔 What is SOQL?

**SOQL** stands for **Salesforce Object Query Language**.

It is used to query data in your Salesforce org using `SELECT` statements — similar to how SQL works.

> 💬 Think of SOQL as **"SQL for Salesforce"** — familiar syntax, tailored for the Salesforce platform.

---

## ❓ Why do we need SOQL?

| 🎯 Purpose | 📝 Description |
|---|---|
| 🗄️ Database Communication | Talk to the Salesforce Database and retrieve exactly what you need |
| 🔗 Flexible Retrieval | Retrieve data from a **single object** or **multiple related objects** |
| 📊 Data Aggregation | **Count, Sort, and Group** records based on criteria |
| 🗂️ All Datatypes | Works with dates, checkboxes, numbers, and more |

---

## 🏗️ Query Structure

```sql
SELECT fieldName1, fieldName2, ...
FROM ObjectName
WHERE condition
```

> ⚠️ **Mandatory:** `SELECT ... FROM ObjectName` is required in every SOQL query.

### 📋 Full Clause Order

```
SELECT ▶ FROM ▶ WHERE ▶ GROUP BY ▶ HAVING ▶ ORDER BY ▶ LIMIT ▶ OFFSET
```

---

## 🔍 Querying Fields

### 🏷️ Standard Fields

Query all Accounts displaying Billing Address:

```sql
SELECT Id, BillingStreet, BillingCity, BillingState, BillingPostalCode, BillingCountry
FROM Account
```

### 🛠️ Custom Fields

Custom fields always use the `__c` suffix:

```sql
SELECT Id, Contact_Full_Name__c, Type__c, Website__c, Number_of_Tasks_Associated__c
FROM Contact
```

> 💡 **Tip:** Any field ending in `__c` is a custom field created by your org's admin.

---

## ✅ Use Cases with WHERE Clause

| 🎯 Use Case | 💻 SOQL Query |
|---|---|
| 🎂 Find Contacts whose birthday is Today | `SELECT Id, Name, Birthdate FROM Contact WHERE Birthdate = Today` |
| 🔥 Publicly owned Accounts with Hot Rating | `SELECT Id, Name, Ownership, Rating FROM Account WHERE Rating = 'Hot' AND Ownership = 'Public'` |
| 🌐 Working-Contacted Leads from Web | `SELECT Name, LeadSource, Status FROM Lead WHERE LeadSource = 'Web' AND Status = 'Working - Contacted'` |
| 👤 Contacts whose FirstName is Lewis | `SELECT FirstName, LastName FROM Contact WHERE FirstName = 'Lewis'` |
| 🏦 Accounts in Banking Industry | `SELECT Name, Industry FROM Account WHERE Industry = 'Banking'` |

---

## 📏 Governor Limits

> 🚦 Salesforce enforces these limits to ensure platform performance for all users.

| 📊 Limit | 🔢 Value |
|---|---|
| ⚡ Max SOQL queries per transaction (synchronous) | **100** |
| 📦 Max records returned per SOQL query | **50,000** |

---

<div align="center">

### 🚀 Happy Querying!

*Built with ❤️ for Salesforce Developers*

</div>
