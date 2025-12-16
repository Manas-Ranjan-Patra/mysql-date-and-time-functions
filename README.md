# MySQL Date & Time Functions 📅⏰

## 📌 Overview

This repository provides a **comprehensive overview of MySQL Date and Time functions** with clear explanations and practical SQL examples. It is designed for **students, beginners, and data professionals** who want to understand how MySQL handles date and time values in real-world database queries.

The content is based on structured learning material and covers **fetching current date/time, extracting components, creating dates/times, performing calculations, and formatting outputs**.

---

## 🎯 Objectives

- Understand MySQL date & time data handling
- Learn commonly used MySQL date and time functions
- Perform date/time extraction and calculations
- Format date and time values for reporting

---

## 🛠️ Tech Stack

- **Database:** MySQL
- **Query Language:** SQL
- **Tool:** MySQL Workbench

---

## 📚 Topics Covered

### 1️⃣ Getting Current Date & Time

- `CURDATE()`
- `CURRENT_DATE()`
- `CURRENT_TIME()`
- `NOW()`
- `CURRENT_TIMESTAMP()`
- `SYSDATE()`

```sql
SELECT CURDATE();
SELECT CURRENT_TIME();
SELECT NOW();
```

---

### 2️⃣ Extracting Date & Time Components

- `DATE()`
- `EXTRACT()`
- `YEAR()`
- `QUARTER()`
- `MONTH()`
- `DAY()`
- `DAYOFYEAR()`
- `HOUR()`
- `MINUTE()`
- `SECOND()`

```sql
SELECT YEAR('2025-12-15 13:06:54') AS year;
SELECT DAYNAME('2025-12-15') AS day_name;
```

---

### 3️⃣ Name-Based Functions

- `DAYNAME()`
- `MONTHNAME()`

```sql
SELECT MONTHNAME('2025-12-15');
```

---

### 4️⃣ Creating Date & Time

- `MAKEDATE()`
- `MAKETIME()`

```sql
SELECT MAKEDATE(2025, 70);
SELECT MAKETIME(14, 45, 06);
```

---

### 5️⃣ Date & Time Calculations

- `ADDTIME()`
- `ADDDATE()`
- `DATEDIFF()`
- `TIMEDIFF()`

```sql
SELECT DATEDIFF('2025-12-15', '2025-10-18');
```

---

### 6️⃣ Converting Strings to Date/Time

- `STR_TO_DATE()`

```sql
SELECT STR_TO_DATE('15,12,2025', '%d,%m,%Y');
```

---

### 7️⃣ Formatting Date & Time

- `DATE_FORMAT()`
- `TIME_FORMAT()`

```sql
SELECT DATE_FORMAT('2025-12-15', '%W %d-%M-%Y');
SELECT TIME_FORMAT('15:30:45', '%h:%i %p');
```

---

## ⚠️ Notes

- Invalid dates return **NULL** in MySQL
- Example:

```sql
SELECT DATE_SUB('2017-02-29', INTERVAL -1 DAY);
```

---

## 👨‍💻 Author

**Manas Ranjan Patra**\
GitHub: [Manas-Ranjan-Patra](https://github.com/Manas-Ranjan-Patra)

LinkedIn : [Manas Ranjan Patra](https://www.linkedin.com/in/manas-ranjan-patra-4171b02a9/)

---

## 🚀 Who Should Use This Repo?

- SQL Beginners
- Data Analysts
- Students preparing for exams/interviews
- Anyone working with date/time data in MySQL

---

## ⭐ Support

If you find this repository helpful, don’t forget to **star ⭐ the repo** and share it with others!

Happy Querying! 🚀
