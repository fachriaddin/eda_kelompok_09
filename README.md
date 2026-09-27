# Performa Operasional Dan Emisi Carbon Green Quantum Data Center

Repositori ini berisi analisis data mengenai performa operasional dan emisi karbon pada *Green Quantum Data Center*. Proyek ini disusun untuk memenuhi tugas mata kuliah dengan topik **Cloud Computing**[cite: 5].

## 👥 Anggota Kelompok (Kelompok 09)
1. Fachri Addin Al Fikri (5027261009)[cite: 5]
2. Raaif Mabkhud Nahdi (5027261042)[cite: 5]
3. Qurrataaini Aghnia Sutino (5027261097)[cite: 5]

---

## 📊 Ringkasan Dataset
* **Sumber Data:** [Kaggle - Green Quantum Data Center Operations](https://www.kaggle.com/datasets/zara2099/green-quantum-data-center-operations)[cite: 5]
* **Lisensi:** CC0: Public Domain[cite: 5]
* **Ukuran Dataset:** 1000 baris dan 6 kolom[cite: 5]
* **Kamus Data:**
  | Kolom | Arti | Jenis Variabel | Satuan |
  | :--- | :--- | :--- | :--- |
  | `workload_type` | Jenis beban kerja pusat data[cite: 5] | Kategorik (Nominal) | –[cite: 5] |
  | `energy_source` | Sumber energi utama operasional[cite: 5] | Kategorik (Nominal) | –[cite: 5] |
  | `compute_demand_TFlops` | Besarnya permintaan komputasi[cite: 5] | Numerik (Rasio) | TFLOPs[cite: 5] |
  | `storage_demand_TB` | Kapasitas penyimpanan data[cite: 5] | Numerik (Rasio) | TB[cite: 5] |
  | `network_demand_Gbps` | Tingkat permintaan jaringan[cite: 5] | Numerik (Rasio) | Gbps[cite: 5] |
  | `carbon_emissions_kgCO2` | Jumlah emisi karbon yang dihasilkan[cite: 5] | Numerik (Rasio) | $\text{kgCO}_2$ (ditulis kgCO2)[cite: 5] |

---

## 🚀 Cara Menjalankan Jupyter Notebook

Ikuti langkah-langkah di bawah ini untuk menjalankan berkas Jupyter Notebook (`.ipynb`) pada perangkat Anda:

### 1. Prasyarat (Prerequisites)
Pastikan Anda sudah menginstal **Python** dan manajer paket **pip** di komputer Anda. Anda juga memerlukan pustaka Pandas untuk membaca dataset.

### 2. Instalasi Pustaka (Dependencies)
Buka terminal atau *command prompt*, lalu instal pustaka yang dibutuhkan menggunakan perintah:
```bash
pip install pandas jupyter
