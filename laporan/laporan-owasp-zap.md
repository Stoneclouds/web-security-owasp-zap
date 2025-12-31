# Laporan Praktik Web Security Analysis
## Menggunakan OWASP ZAP

### 1. Pendahuluan
Laporan ini dibuat sebagai bagian dari pembelajaran Cyber Security, khususnya
pada analisis keamanan aplikasi web menggunakan OWASP ZAP.

Pengujian dilakukan pada **OWASP Juice Shop** yang dijalankan secara lokal
di lingkungan pribadi untuk tujuan edukasi.

---

### 2. Tools yang Digunakan
- OWASP ZAP
- OWASP Juice Shop (Localhost)

---

### 3. Metodologi Pengujian
Metode pengujian yang digunakan adalah **Automated Scanning** dengan OWASP ZAP,
yang mencakup proses crawling aplikasi web dan identifikasi potensi celah keamanan
secara otomatis.

Target URL:
https://localhost:3000


---

### 4. Hasil Pengujian
Berdasarkan hasil pemindaian, ditemukan beberapa potensi permasalahan keamanan
pada konfigurasi aplikasi web, antara lain:

#### 4.1 Content Security Policy (CSP) Header Not Set
- **Risk**: Medium
- **Deskripsi**: Aplikasi tidak menerapkan Content Security Policy (CSP) sehingga
  berpotensi meningkatkan risiko serangan Cross-Site Scripting (XSS).
- **Rekomendasi**: Menambahkan header CSP yang sesuai untuk membatasi sumber konten.

#### 4.2 Cross-Domain Misconfiguration
- **Risk**: Medium
- **Deskripsi**: Konfigurasi lintas domain yang kurang tepat dapat membuka akses
  tidak sah dari domain lain.
- **Rekomendasi**: Mengatur kebijakan CORS dengan lebih ketat.

---

### 5. Kesimpulan
Penggunaan OWASP ZAP membantu dalam mengidentifikasi potensi celah keamanan
pada aplikasi web. Hasil pengujian ini menunjukkan pentingnya penerapan
konfigurasi keamanan yang baik sejak tahap pengembangan aplikasi.

---

### 6. Catatan Etika
Seluruh pengujian dilakukan pada lingkungan yang legal dan disengaja rentan
(OWASP Juice Shop) untuk tujuan pembelajaran.
