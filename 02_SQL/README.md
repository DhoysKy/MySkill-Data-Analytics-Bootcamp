# SQL for Data Analysis: Tokopaedi E-Commerce Project 🛒

## 📌 Deskripsi Proyek
Proyek ini merupakan kompilasi dari serangkaian *Mini Tasks* (Task 5 - 9) yang berfokus pada end-to-end proses Data Analysis menggunakan **PostgreSQL**. Proyek ini mensimulasikan peran seorang Data Analyst di sebuah *e-commerce* fiktif bernama Tokopaedi, dimulai dari perancangan arsitektur database awal hingga ekstraksi *business insights* tingkat lanjut.

## 🛠️ Tools & Teknologi
* **Database Management System:** PostgreSQL (pgAdmin 4)
* **Data Preparation:** Google Sheets / Excel
* **Query Language:** SQL (DDL, DML, DQL)

## 📂 Struktur Proyek
Proyek ini didokumentasikan dalam bentuk presentasi (*slide* PowerPoint) yang berisi metodologi, potongan kode (*code snippets*), dan tangkapan layar hasil eksekusi *query*.

### 1. Database & Table Creation (DDL)
* Membuat wadah database `tokopaedi`.
* Merancang skema tabel `orders` dengan pemilihan tipe data yang presisi (seperti `VARCHAR`, `FLOAT` untuk finansial, dan `DATE` untuk *time-series*) guna mengoptimalkan memori dan menjaga integritas data.

### 2. Data Cleaning & Import Data
* Melakukan standarisasi format data finansial (menghilangkan pemisah ribuan) pada sumber *file* CSV.
* Melakukan proses *importing* ribuan baris data mentah ke dalam PostgreSQL tanpa adanya *data corruption*.

### 3. Data Filtering & Sorting (Basic SQL)
* **Filtering Spesifik:** Menggunakan klausa `WHERE`, `AND`, dan `IN` untuk mengidentifikasi segmen pelanggan tertentu (misal: konsumen B2B di wilayah spesifik).
* **Date Extraction:** Mengekstrak elemen waktu (Tahun/Kuartal) menggunakan fungsi `EXTRACT()` untuk menganalisis tren pada periode waktu tertentu (contoh: Kuartal 1 2018).
* **Sorting:** Mengurutkan transaksi paling menguntungkan dan merugikan menggunakan `ORDER BY ... ASC/DESC`.

### 4. Advanced SQL Analysis
Menggunakan fungsi Agregasi, Common Table Expressions (CTE), dan Subqueries untuk mengeksekusi logika bisnis yang kompleks:
* Memvalidasi integritas data (Rasio 1:1 antara Nama Konsumen dan *Customer ID*) menggunakan `GROUP BY` dan `HAVING`.
* Mengidentifikasi *Best-Selling Product* berdasarkan kuantitas (`SUM`).
* Menentukan "Top City" penyumbang *revenue* tertinggi.
* **Customer Segmentation:** Menganalisis rata-rata pengeluaran konsumen di suatu kota, dan mengidentifikasi daftar pelanggan "High-Value" (di atas rata-rata) menggunakan *Subqueries* dan klausa `WITH` (CTE).

## 🚀 Kesimpulan
Melalui proyek ini, jutaan kemungkinan dari data transaksi berhasil disaring menjadi wawasan bisnis yang siap ditindaklanjuti, membuktikan bahwa SQL bukan hanya sekadar alat penyimpan data, melainkan instrumen analitik yang sangat tajam.
