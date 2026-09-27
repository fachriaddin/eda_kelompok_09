# Proyek 1: Eksplorasi Data (Exploratory Data Analysis)
## Mata Kuliah: Statistika dan Probabilitas (ET234101)

Repositori ini disusun untuk memenuhi tugas **Proyek 1: Eksplorasi Data**. Fokus dari proyek ini adalah melakukan pengenalan awal terhadap data (*Exploratory Data Analysis* / EDA) yang meliputi pemahaman struktur data, pengecekan data kosong, statistik deskriptif, serta visualisasi data awal tanpa menggunakan uji hipotesis atau *machine learning*.

## 👥 Anggota Kelompok (Kelompok 09)
1. **Fachri Addin Al Fikri** (5027261009)
2. **Raaif Mabkhud Nahdi** (5027261042)
3. **Qurrataaini Aghnia Sutino** (5027261097)

---

## 📊 Informasi Dataset
* **Topik Pilihan:** Cloud (Infrastruktur dan Layanan Komputasi Awan)
* **Sumber Data:** [Kaggle - Green Quantum Data Center Operations](https://www.kaggle.com/datasets/zara2099/green-quantum-data-center-operations)
* **Ukuran Dataset:** 1000 baris dan 6 kolom
* **Kamus Data:**
  | Kolom | Arti / Deskripsi | Jenis Variabel | Satuan |
  | :--- | :--- | :--- | :--- |
  | `workload_type` | Jenis beban kerja pusat data | Kategorik (Nominal) | – |
  | `energy_source` | Sumber energi utama operasional | Kategorik (Nominal) | – |
  | `compute_demand_TFlops` | Besarnya permintaan komputasi | Numerik (Rasio) | TFLOPs |
  | `storage_demand_TB` | Kapasitas penyimpanan data | Numerik (Rasio) | TB |
  | `network_demand_Gbps` | Tingkat permintaan jaringan | Numerik (Rasio) | Gbps |
  | `carbon_emissions_kgCO2` | Jumlah emisi karbon yang dihasilkan | Numerik (Rasio) | $\text{kgCO}_2$ (kgCO2) |

---

## 📋 Tahap Pengerjaan Proyek
1. **Cek Anggota Kelompok:** Bergabung ke dalam grup komunikasi dengan anggota kelompok yang telah dibagi secara acak melalui [Tautan Pembagian Kelompok](https://docs.google.com/spreadsheets/d/1DYGqZP-cE1R45a5qWif2PWlgk_qH0jmYWobGNppLXaE/edit?usp=sharing).
2. **Tentukan Topik dan Cari Dataset:** Memilih topik *Cloud* dan mengunduh dataset publik dari Kaggle yang memenuhi kriteria (minimal 200 baris, 5 kolom, format CSV/Excel di bawah 25 MB).
3. **Siapkan Miniconda dan Jupyter Notebook:** Menyiapkan lingkungan lokal secara mandiri tanpa menggunakan Google Colab atau asisten AI otomatis agar terbiasa menulis sintaks Python.
4. **Kerjakan EDA di Notebook:** Melakukan eksplorasi data, pengecekan nilai kosong, statistik deskriptif, dan visualisasi grafik sesuai struktur yang ditentukan.
5. **Unggah ke GitHub:** Mengunggah *notebook* (`.ipynb`), dataset, dan berkas `README.md` ini ke repositori kelompok, lalu mengumpulkan tautannya di myITS Learning.
6. **Demo di Kelas (Minggu ke-5):** Menjalankan *notebook* di depan kelas dan menjawab pertanyaan dosen.

---

## 🚀 Panduan Instalasi & Menjalankan Jupyter Notebook (Lokal)

Pengerjaan dilakukan secara lokal menggunakan **Miniconda** dan **Jupyter Notebook** dengan langkah-langkah berikut:

### Langkah 1: Unduh dan Install Miniconda
1. Unduh installer Miniconda melalui halaman resmi sesuai sistem operasi Anda.
2. Untuk pengguna Windows, buka installer, pilih opsi **Just Me**, dan gunakan pengaturan bawaan (*default*).

### Langkah 2: Buat Environment Khusus Mata Kuliah
Buka **Anaconda Prompt** (untuk Windows) atau **Terminal** (untuk macOS/Linux), lalu jalankan perintah berikut untuk membuat *environment* baru bernama `statprob`:
```bash
conda create -n statprob python=3.11 -y
conda activate statprob
conda install -c conda-forge jupyter pandas matplotlib seaborn -y
cd lokasi/folder/proyek1
jupyter notebook
