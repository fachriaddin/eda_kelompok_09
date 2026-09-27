# Analisis Eksplorasi Data (EDA): Green Quantum Data Center Operations
## Proyek 1: Statistika dan Probabilitas (ET234101)

Repositori ini berisi laporan dan dokumentasi mendalam mengenai eksplorasi data (*Exploratory Data Analysis* / EDA) pada operasional *Green Quantum Data Center*. Proyek ini bertujuan untuk mengenali karakteristik data, memeriksa kualitas data, serta memahami pola sebaran dan hubungan antarvariabel sebelum melangkah ke tahap pemodelan lanjutan.

## 🎯 Latar Belakang & Tujuan Proyek
Pusat data (*data center*) modern membutuhkan pengelolaan sumber daya komputasi dan energi yang efisien untuk menekan dampak lingkungan. Melalui proyek ini, dilakukan analisis terhadap dataset operasional pusat data untuk menjawab beberapa pertanyaan mendasar:
1. Bagaimana distribusi beban kerja (*workload*) dan penggunaan sumber energi di pusat data?
2. Bagaimana karakteristik statistik dari permintaan komputasi, penyimpanan, jaringan, dan emisi karbon?
3. Apakah terdapat kaitan atau pola antara variabel-variabel operasional tersebut?

---

## 📂 Struktur Dataset
* **Sumber Data:** [Kaggle - Green Quantum Data Center Operations](https://www.kaggle.com/datasets/zara2099/green-quantum-data-center-operations)
* **Dimensi Data:** 1000 baris dan 6 kolom
* **Kamus Data:**
  | Kolom | Deskripsi Variabel | Jenis Data | Satuan |
  | :--- | :--- | :--- | :--- |
  | `workload_type` | Jenis beban kerja pusat data (misal: AI Training, Cloud Hosting, dll.) | Kategorik (Nominal) | – |
  | `energy_source` | Sumber energi utama yang digunakan (misal: Solar, Wind, Grid, dll.) | Kategorik (Nominal) | – |
  | `compute_demand_TFlops` | Besarnya permintaan daya komputasi | Numerik (Rasio) | TFLOPs |
  | `storage_demand_TB` | Kapasitas penyimpanan data yang dialokasikan | Numerik (Rasio) | TB |
  | `network_demand_Gbps` | Tingkat kebutuhan bandwidth / jaringan | Numerik (Rasio) | Gbps |
  | `carbon_emissions_kgCO2` | Jumlah emisi karbon yang dihasilkan dari operasional | Numerik (Rasio) | $\text{kgCO}_2$ |

---

## 🔍 Tahapan Analisis dalam Notebook (`.ipynb`)
Proyek ini dieksplorasi secara sistematis melalui beberapa tahapan utama di dalam Jupyter Notebook:

1. **Pemuatan Data (*Data Loading*):**
   * Membaca dataset format CSV menggunakan pustaka `pandas`.
   * Menampilkan beberapa baris pertama data (`df.head()`), ukuran data, serta tipe data masing-masing kolom.

2. **Pembersihan Data (*Data Cleaning*):**
   * Memeriksa keberadaan nilai yang hilang (*missing values*), data duplikat, atau anomali data (*outliers*) yang dapat memengaruhi keakuratan analisis.

3. **Statistika Deskriptif:**
   * **Ukuran Pemusatan:** Menghitung nilai rata-rata (*mean*) dan nilai tengah (*median*) untuk variabel numerik seperti permintaan komputasi dan emisi karbon.
   * **Ukuran Penyebaran:** Menghitung nilai minimum, maksimum, rentang (*range*), serta standar deviasi untuk melihat variasi data.
   * **Analisis Frekuensi:** Merekapitulasi sebaran kategori pada kolom `workload_type` dan `energy_source`.

4. **Visualisasi Data:**
   * Menggunakan `matplotlib` dan `seaborn` untuk menyajikan grafik yang informatif, seperti:
     * *Histogram* dan *Boxplot* untuk melihat distribusi dan sebaran nilai numerik.
     * *Bar Chart* atau *Count Plot* untuk membandingkan frekuensi kategori beban kerja dan sumber energi.
     * *Scatter Plot* untuk melihat potensi hubungan antara variabel numerik (misalnya permintaan komputasi terhadap emisi karbon).

---

## 📌 Kesimpulan & Temuan Awal
* Berdasarkan eksplorasi awal, data bersih dari nilai kosong yang signifikan dan siap digunakan untuk analisis lanjutan.
* Variabel numerik menunjukkan variasi yang baik, memenuhi kriteria untuk analisis statistik deskriptif dan persiapan Proyek Akhir (regresi).
