# SQL Injection Vulnerability in WHERE Clause Allowing Retrieval of Hidden Data

## Lab Information

* Platform: PortSwigger Web Security Academy
* Category: SQL Injection
* Difficulty: Apprentice

---

## Objective

Memanfaatkan SQL Injection pada klausa WHERE untuk menampilkan data yang seharusnya tidak dapat diakses oleh pengguna.

---

## Vulnerability Overview

Aplikasi menggunakan input pengguna secara langsung dalam query SQL tanpa validasi yang memadai.

Hal ini memungkinkan penyerang memodifikasi kondisi WHERE sehingga data tersembunyi dapat ditampilkan.

---

## Testing Process

### Step 1

Mengidentifikasi parameter yang digunakan untuk memfilter data.

### Step 2

Melakukan pengujian terhadap parameter dengan karakter khusus SQL.

### Step 3

Mengamati perubahan hasil yang ditampilkan aplikasi.

### Step 4

Memodifikasi kondisi query sehingga seluruh data dapat ditampilkan.

---

## Result

Lab berhasil diselesaikan dan data tersembunyi berhasil ditampilkan.

---

## Security Impact

* Akses tidak sah terhadap data
* Kebocoran informasi
* Bypass logika aplikasi

---

## Mitigation

* Prepared Statements
* Parameterized Queries
* Input Validation

---

## OWASP Top 10 Mapping

A03:2021 - Injection

---

## Learning Notes

Lab ini membantu memahami bagaimana manipulasi klausa WHERE dapat menyebabkan kebocoran data.

