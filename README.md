# Analisis Efektivitas Pembelajaran Online (Online Learning Effectiveness Analysis)

Repositori ini berisi proyek praktikum *Machine Learning* yang bertujuan untuk menganalisis faktor-faktor yang memengaruhi performa akademik mahasiswa dalam pembelajaran online. Dataset yang digunakan berisi informasi mengenai durasi belajar daring, keterlibatan mahasiswa, kehadiran kelas, kualitas koneksi internet, perangkat yang digunakan, serta tingkat kepuasan belajar.

---

## 📋 Daftar Isi
1. [Tentang Proyek](#tentang-proyek)
2. [Struktur Dataset](#struktur-dataset)
3. [Alur Kerja (Workflow)](#alur-kerja-workflow)
4. [Instalasi dan Kebutuhan Sistem](#instalasi-dan-kebutuhan-sistem)
5. [Cara Menjalankan Proyek](#cara-menjalankan-proyek)
6. [Hasil dan Evaluasi Model](#hasil-dan-evaluasi-model)
7. [Kontributor](#kontributor)

---

## 🎯 Tentang Proyek
Pembelajaran online menjadi bagian penting dalam dunia pendidikan modern. Dalam konteks ini, mahasiswa menghadapi berbagai faktor yang dapat memengaruhi keberhasilan belajar, seperti keterlibatan belajar, kehadiran di kelas online, kualitas internet, serta beban kerja yang mereka rasakan. Proyek ini menggunakan pendekatan *Supervised Learning* dengan tipe **Regresi** untuk memprediksi nilai GPA mahasiswa berdasarkan variabel-variabel tersebut.

Target utama dalam model adalah `Academic_Performance_GPA`, yaitu nilai akademik numerik yang diprediksi dari fitur pembelajaran digital.

---

## 📊 Struktur Dataset
Dataset yang digunakan dalam proyek ini adalah `online_learning_effectiveness_dataset.csv`, yang mencakup berbagai variabel, antara lain:
* **Fitur Demografi**: usia, gender, level akademik
* **Fitur Pembelajaran Online**: platform belajar, durasi belajar harian, persentase kehadiran kelas, perangkat yang digunakan
* **Fitur Kualitas Belajar**: skor keterlibatan, tingkat interaksi, stabilitas internet, tingkat beban kerja, tingkat kepuasan belajar
* **Variabel Target (`Academic_Performance_GPA`)**: nilai GPA mahasiswa yang bersifat numerik

---

## 🔄 Alur Kerja (Workflow)
Notebook ini dirancang secara sistematis melalui beberapa tahapan utama:
1. **Pemuatan Dataset & Eksplorasi Awal (EDA)**: memuat data, melihat struktur, tipe data, serta jumlah missing value.
2. **Analisis Korelasi**: mengecek hubungan antar fitur numerik dan melihat variabel yang paling berpengaruh terhadap GPA.
3. **Preprocessing Data**: menangani missing value, melakukan encoding pada data kategorikal, serta scaling untuk fitur numerik.
4. **Pembagian Data**: membagi data menjadi data latih dan data uji dengan rasio 80:20.
5. **Pemodelan**: membangun model regresi menggunakan `LinearRegression` dan membandingkannya dengan `RandomForestRegressor`.
6. **Evaluasi Model**: menguji performa model menggunakan metrik MAE, RMSE, dan R².
7. **Interpretasi Hasil**: menilai faktor yang paling berpengaruh terhadap efektivitas pembelajaran online.

---

## 🛠️ Instalasi dan Kebutuhan Sistem
Pastikan Anda telah menginstal Python (disarankan versi 3.8 ke atas) beserta pustaka-pustaka berikut:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## 🚀 Cara Menjalankan Proyek
1. Clone atau unduh repositori ini ke komputer lokal Anda.
2. Masuk ke direktori proyek:
   ```bash
   cd Tugas-Machine-Learning
   ```
3. Pastikan file dataset `online_learning_effectiveness_dataset.csv` ada di folder yang sama dengan notebook.
4. Buka Jupyter Notebook atau JupyterLab:
   ```bash
   jupyter notebook main.ipynb
   ```
5. Jalankan sel secara berurutan dari atas ke bawah.

---

## 📈 Hasil dan Evaluasi Model
* **Model yang Digunakan**: `LinearRegression` dan `RandomForestRegressor`
* **Metrik Evaluasi**:
  * `MAE` (Mean Absolute Error)
  * `RMSE` (Root Mean Squared Error)
  * `R²` (Coefficient of Determination)
* **Tujuan Evaluasi**: mengetahui model manakah yang paling sesuai untuk memprediksi GPA berdasarkan faktor pembelajaran online.

---

## 👥 Kontributor
Proyek ini dikembangkan untuk keperluan tugas praktikum *Machine Learning* dengan fokus pada analisis efektivitas pembelajaran online. Silakan gunakan sebagai referensi untuk mengembangkan analisis lebih lanjut dan tetap menjaga orisinalitas pekerjaan.
