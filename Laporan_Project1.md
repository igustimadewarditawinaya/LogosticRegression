# Laporan Proyek Machine Learning - I Gusti Made Wardita Winaya 

## Domain Proyek
Pada era digital saat ini, data dari media sosial dapat digunakan untuk memahami perilaku pengguna dan membuat keputusan bisnis yang lebih baik. Salah satu aplikasi dari Machine Learning adalah dalam menentukan apakah seorang pengguna akan membeli suatu produk berdasarkan atribut tertentu. Dalam proyek ini, kami menggunakan algoritma **Logistic Regression** untuk melakukan klasifikasi terhadap data pengguna dari dataset **Social_Network_Ads.csv**.

### Mengapa Masalah Ini Harus Diselesaikan?
Dengan memprediksi kemungkinan seorang pengguna membeli produk, bisnis dapat mengoptimalkan strategi pemasaran dan meningkatkan konversi pelanggan. Logistic Regression adalah salah satu metode yang efektif untuk menangani masalah klasifikasi biner seperti ini.

## Business Understanding

### Problem Statements
1. Bagaimana cara mengklasifikasikan pengguna berdasarkan fitur-fitur yang tersedia dalam dataset?
2. Seberapa akurat model Logistic Regression dalam memprediksi pembelian pengguna?

### Goals
1. Mengembangkan model klasifikasi yang dapat memprediksi apakah seorang pengguna akan melakukan pembelian.
2. Mengevaluasi performa model menggunakan metrik yang sesuai seperti akurasi, precision, recall, dan F1-score.

### Solution Statements
Untuk mencapai tujuan di atas, kami menerapkan **Logistic Regression** sebagai algoritma utama dalam klasifikasi data. Selain itu, kami akan:
- Membagi data menjadi **training** dan **testing set**.
- Melakukan **feature scaling** untuk meningkatkan performa model.
- Menggunakan **evaluasi metrik** yang relevan untuk menilai performa model.

## Data Understanding
Dataset yang digunakan adalah **Social_Network_Ads.csv**, yang terdiri dari beberapa variabel:
- **User ID**: Identifikasi unik pengguna (tidak digunakan dalam pemodelan).
- **Age**: Usia pengguna.
- **Estimated Salary**: Perkiraan gaji pengguna.
- **Purchased**: Label target (1 jika membeli, 0 jika tidak).

Kami melakukan eksplorasi data untuk memahami distribusi fitur dan korelasi antar variabel menggunakan visualisasi data.

## Data Preparation
Sebelum membangun model, kami melakukan beberapa tahap preprocessing:
1. **Membagi dataset** menjadi **training set (75%)** dan **testing set (25%)**.
2. **Melakukan Feature Scaling** menggunakan **StandardScaler** dari Scikit-Learn untuk menormalkan fitur numerik.

## Modeling
Dalam proyek ini, kami menggunakan **Logistic Regression** sebagai algoritma utama. Proses pemodelan melibatkan:
- Inisialisasi model Logistic Regression dari **Scikit-Learn**.
- Pelatihan model menggunakan data training.
- Memprediksi hasil pada data testing.

**Kelebihan Logistic Regression:**
- Sederhana dan mudah diinterpretasikan.
- Tidak memerlukan banyak sumber daya komputasi.
- Cocok untuk klasifikasi biner.

**Kekurangan Logistic Regression:**
- Kurang efektif untuk dataset dengan hubungan non-linear yang kompleks.
- Rentan terhadap outlier.

## Evaluation
Kami menggunakan beberapa metrik evaluasi untuk mengukur performa model, termasuk:
- **Akurasi**: Mengukur seberapa sering prediksi model benar.
- **Precision**: Mengukur seberapa tepat model dalam mengklasifikasikan kelas positif.
- **Recall**: Mengukur seberapa baik model dalam menangkap semua instance positif.
- **F1-Score**: Rata-rata harmonik dari precision dan recall.

Hasil evaluasi menunjukkan bahwa Logistic Regression memberikan performa yang cukup baik dalam menyelesaikan masalah klasifikasi ini. Jika diperlukan peningkatan performa, dapat dilakukan **hyperparameter tuning** atau mencoba model lain seperti **SVM atau Random Forest**.

---
Laporan ini memberikan pemahaman yang jelas tentang bagaimana Logistic Regression dapat diterapkan dalam kasus klasifikasi data pengguna media sosial. Dengan hasil yang diperoleh, bisnis dapat menggunakan model ini untuk mendukung keputusan pemasaran yang lebih strategis.

