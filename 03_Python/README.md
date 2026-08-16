# 🐍 Python for Data Analysis: Fundamentals to Data Visualization

## 📌 Deskripsi Proyek
Selamat datang di direktori Python! Bagian ini mendemonstrasikan transisi dari pemahaman sintaks dasar Python (*Data Structures*) menuju manipulasi data tingkat lanjut menggunakan *library* andalan Data Analyst: **Pandas** dan **Matplotlib**. 

Proyek ini merangkum *Mini Tasks* (Task 10 & 11) di mana saya mengeksekusi logika pemrograman dasar hingga membedah dan memvisualisasikan dataset nyata mengenai tren Imigrasi Kanada (*Canada Immigration Dataset*).

## 🛠️ Tools & Teknologi
* **Programming Language:** Python 3
* **Libraries:** Pandas (Data Manipulation), Matplotlib (Data Visualization)
* **Environment:** Google Colaboratory / Jupyter Notebook

---

## 🗂️ Rincian Proyek & Portfolio

### 1️⃣ Python Fundamentals: Interactive Dictionary
📄 **File:** `Mini Task 10 - Basic Python.pptx`

Sebelum mengolah jutaan baris data, seorang analis harus menguasai struktur data fundamental. Pada tugas ini, saya merancang program biodata interaktif dengan menonjolkan penulisan kode yang *Pythonic* dan anti-*error*:
* **Interactive Data Entry:** Memanfaatkan fungsi `input()` dipadukan dengan *Looping* untuk membangun dan menampilkan form *Dictionary* secara dinamis dan rapi.
* **Error-Safe Extraction:** Meninggalkan pemanggilan *key* menggunakan kurung siku konvensional dan beralih ke metode `.get()` untuk mencegah *program crash* (*KeyError*) jika data tidak ditemukan.
* **Advanced String Formatting:** Mengimplementasikan teknik *Dictionary Unpacking* (`**`) untuk mengekstrak dan menyuntikkan berbagai *value* secara otomatis ke dalam sebuah kalimat dengan sintaks yang elegan.

### 2️⃣ Data Manipulation & Cleansing (Pandas)
📄 **File:** `Mini Task 11 - Data Analysis Study case.pptx`

Fase persiapan data (*Data Preparation*) sebelum melakukan analisis mendalam. Pada bagian ini, saya menggunakan `Pandas` untuk membentuk ulang struktur *dataframe*:
* **Column Standardization:** Mengubah nama kolom yang kurang deskriptif (seperti `REG` dan `DEV`) menjadi lebih intuitif menggunakan fungsi `.rename()` dan teknik *Dictionary*.
* **Data Subsetting:** Memotong *dataframe* berukuran besar hanya pada kolom-kolom spesifik yang relevan dengan tujuan bisnis (contoh: hanya mengambil kolom Negara, Benua, dan Tahun 2013).
* **Boolean Indexing & Locating:** Mengekstrak baris data spesifik (contoh: Negara Andorra) menggunakan filter logika dasar dan identifikasi indeks tingkat lanjut dengan fungsi `.loc[]`.

### 3️⃣ Exploratory Data Analysis (EDA) & Visualization
📄 **File:** `Mini Task 11 - Data Analysis Study case.pptx`

Tahap krusial untuk menjawab pertanyaan bisnis: *"Bandingkan tren dari 5 negara penyumbang imigran terbanyak ke Kanada"*. Saya mengeksekusi analisis *end-to-end* dengan langkah berikut:
* **Method Chaining:** Menggabungkan fungsi *Filtering* (Benua Eropa), *Sorting* (diurutkan dari total imigran terbesar menggunakan `.sort_values(ascending=False)`), dan *Subsetting* secara efisien dalam satu baris kode (*one-liner code*).
* **Data Restructuring:** Menerapkan fungsi `.transpose()` untuk memutar tabel data waktu (*time-series*), memastikan sumbu X (Tahun) dan garis grafik (Negara) dapat dibaca dengan benar oleh sistem.
* **Data Visualization:** Merancang grafik garis (*Multi-line chart*) interaktif menggunakan `Matplotlib`. Grafik dioptimalkan dengan resolusi yang tepat (`figsize`), serta penambahan elemen informatif seperti *Title*, *X-label*, *Y-label*, dan *Legend*.

## 🚀 Kesimpulan
Melalui modul ini, saya membuktikan kemampuan untuk menerjemahkan logika bisnis ke dalam baris kode Python. Mulai dari pembersihan tabel mentah menggunakan Pandas hingga menghasilkan *insight* visual melalui Matplotlib yang siap dipresentasikan kepada *stakeholders*.
```eof

Silakan buat file baru bernama `README.md` di dalam folder `python` GitHub Anda, lalu *paste* seluruh kode di atas. GitHub akan otomatis me- *render* tulisan tersebut menjadi tampilan portofolio yang sangat rapi!
