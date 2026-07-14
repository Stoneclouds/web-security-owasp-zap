# SQL Injection Vulnerability Allowing Login Bypass

## Lab Information

* Platform: PortSwigger Web Security Academy
* Category: SQL Injection
* Difficulty: Apprentice

---

## Objective

Memanfaatkan SQL Injection untuk melewati proses autentikasi dan masuk tanpa kredensial yang valid.

---

## Vulnerability Overview

Input login digunakan langsung dalam query autentikasi tanpa mekanisme sanitasi yang memadai.

---

## Testing Process

### Step 1

Mengidentifikasi form login.

### Step 2

Melakukan pengujian terhadap field autentikasi.

### Step 3

Mengamati respons aplikasi.

### Step 4

Melakukan bypass autentikasi.

---

## Result

Lab berhasil diselesaikan dan autentikasi berhasil dilewati.

---

## Security Impact

* Unauthorized Access
* Privilege Escalation
* Data Exposure

---

## Mitigation

* Prepared Statements
* Parameterized Queries
* Secure Authentication Design

---

## OWASP Top 10 Mapping

A03:2021 - Injection

---

## Learning Notes

Lab ini memperkenalkan konsep Authentication Bypass menggunakan SQL Injection.

