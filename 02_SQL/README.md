# 🗄️ SQL for Data Analysis: Tokopaedi E-Commerce Project

## 📌 Deskripsi Proyek
Selamat datang di direktori SQL! Bagian ini berfokus pada kekuatan transformasi data relasional, mendemonstrasikan bagaimana jutaan baris data mentah dapat dijinakkan dan diolah menjadi wawasan bisnis yang siap ditindaklanjuti menggunakan **PostgreSQL**.

Di sini, saya mensimulasikan peran seorang Data Analyst di sebuah *e-commerce* fiktif bernama Tokopaedi. Proyek ini merangkum serangkaian *Mini Tasks* (Task 5 - 9), di mana saya mengeksekusi proses *end-to-end* mulai dari perancangan arsitektur database awal (DDL), pembersihan dan validasi data, hingga ekstraksi *insight* tingkat lanjut menggunakan fungsi agregasi dan *Subqueries*.

## 🛠️ Tools & Teknologi
* **Database Management System:** PostgreSQL (pgAdmin 4)
* **Data Preparation:** Google Sheets / Microsoft Excel
* **Query Language:** SQL (DDL, DML, DQL)

---

## 🗂️ Rincian Proyek & Portfolio
Proyek ini didokumentasikan dalam bentuk presentasi (*slide* PowerPoint) yang berisi metodologi, potongan kode (*code snippets*), dan tangkapan layar hasil eksekusi *query*.

### 1️⃣ Database Architecture & Table Creation (DDL)
📄 **File:** `Mini Task 5 - Database Creation.pptx`

Sebelum data masuk, sebuah sistem penyimpanan yang kokoh harus dibangun. Pada bagian ini, saya berfokus pada:
* **Database Setup:** Membuat wadah database utama bernama `tokopaedi`.
* **Schema Design:** Merancang skema tabel `orders` dengan pemilihan tipe data yang presisi (seperti `VARCHAR` untuk teks ID, `FLOAT` untuk nilai finansial agar presisi, dan `DATE` untuk format penanggalan) guna mengoptimalkan memori server dan menjaga integritas data.

### 2️⃣ Data Cleansing & Import Process
📄 **File:** `Mini Task 6 - Import Data.pptx`

Memastikan data dari sumber luar siap dikonsumsi oleh database relasional:
* **Format Standardization:** Melakukan standarisasi format data finansial (menghilangkan pemisah ribuan/koma) pada sumber file `.csv` mentah agar sesuai dengan standar sistem SQL.
* **Data Importing:** Mengeksekusi proses *importing* ribuan baris data transaksi ke dalam PostgreSQL secara akurat tanpa adanya *data corruption*.

### 3️⃣ Data Extraction, Filtering & Sorting (DQL)
📄 **File:** `Mini Task 7 & 8 - Basic SQL.pptx`

Mengubah lautan data menjadi informasi spesifik menggunakan perintah kueri dasar:
* **Specific Filtering:** Menggunakan klausa `WHERE`, `AND`, dan `IN` untuk mengidentifikasi segmen pelanggan tertentu (contoh: menemukan konsumen tipe *Corporate* di negara bagian tertentu).
* **Time-Series Extraction:** Mengekstrak elemen waktu menggunakan fungsi `EXTRACT()` untuk menganalisis tren performa pada periode tertentu (contoh: performa kuartal pertama tahun 2018).
* **Data Sorting:** Mengurutkan daftar transaksi paling menguntungkan dan paling merugikan untuk prioritas evaluasi bisnis menggunakan `ORDER BY ... ASC/DESC`.

### 4️⃣ Advanced Business Analysis (Aggregation & Subqueries)
📄 **File:** `Mini Task 9 - Advanced SQL.pptx`

Mengeksekusi logika bisnis yang kompleks untuk menjawab pertanyaan strategis perusahaan menggunakan fungsi agregasi, *Common Table Expressions* (CTE), dan *Subqueries*:
* **Data Validation:** Memvalidasi rasio 1:1 antara Nama Konsumen dan *Customer ID* menggunakan kombinasi `GROUP BY` dan `HAVING`.
* **Performance Metrics:** Mengidentifikasi *Best-Selling Product* (berdasarkan `SUM` kuantitas) dan menentukan "Top City" penyumbang *revenue* tertinggi perusahaan.
* **Customer Segmentation:** Menganalisis rata-rata pengeluaran konsumen di suatu kota, dan mengkategorikan daftar pelanggan "*High-Value*" (pembelanjaan di atas rata-rata) menggunakan klausa `WITH` (CTE) dipadukan dengan *Subqueries*.

---

## 🚀 Kesimpulan
Melalui proyek ini, jutaan kemungkinan dari data transaksi mentah berhasil disaring menjadi wawasan bisnis yang siap ditindaklanjuti. Ini membuktikan bahwa SQL bukan hanya sekadar alat penyimpanan data, melainkan instrumen analitik yang sangat tajam untuk mendukung pengambilan keputusan.
