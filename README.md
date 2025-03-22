# PCA-FA-Diabetes-Analysis-R

Kode ini dirancang untuk melakukan analisis *Principal Component Analysis (PCA)* dan *Factor Analysis (FA)* pada dataset *diabetes.csv* menggunakan bahasa pemrograman R. Dengan menggunakan metode PCA dan FA, kode ini membantu memahami pola dalam data dengan mengurangi dimensi dan mengeksplorasi hubungan antar variabel.

## Fitur Utama

1. **Pre-processing Data**
   - Membaca dataset *diabetes.csv* dan melakukan pengecekan data yang hilang.
   - Mengecek matriks korelasi dan melakukan uji *Kaiser-Meyer-Olkin (KMO)* serta *Bartlett's Test*.

2. **Principal Component Analysis (PCA)**
   - Menghitung *eigenvalues* dan *eigenvectors* secara manual.
   - Menampilkan proporsi varians yang dijelaskan oleh masing-masing komponen utama.
   - Menggunakan fungsi `prcomp` dan `FactoMineR` untuk membandingkan hasil PCA.
   - Visualisasi hasil PCA dengan *scree plot*, *biplot*, dan *correlation circle*.

3. **Factor Analysis (FA)**
   - Menghitung faktor berdasarkan matriks kovarians.
   - Menentukan *factor loadings* untuk tiga faktor utama.
   - Menampilkan diagram faktor untuk memahami hubungan antar variabel.

## Cara Menggunakan

1. Clone repositori ini:
   ```bash
   git clone https://github.com/username/PCA-FA-Diabetes-Analysis-R.git
   ```

2. Masuk ke direktori proyek:
   ```bash
   cd PCA-FA-Diabetes-Analysis-R
   ```

3. Pastikan Anda memiliki R dan pustaka yang diperlukan:
   ```r
   install.packages(c("psych", "dplyr", "FactoMineR", "factoextra", "gridExtra"))
   ```

4. Jalankan skrip R untuk melakukan analisis:
   ```r
   source("analysis.R")
   ```

## Struktur Dataset

Dataset yang digunakan dalam analisis ini memiliki beberapa kolom yang mencakup berbagai parameter medis terkait diabetes. Struktur dataset terdiri dari:
- **Glucose**: Kadar glukosa dalam darah.
- **BloodPressure**: Tekanan darah pasien.
- **SkinThickness**: Ketebalan lipatan kulit.
- **Insulin**: Kadar insulin dalam tubuh.
- **BMI**: Indeks Massa Tubuh.
- **Age**: Usia pasien.
- **Outcome**: Klasifikasi diabetes (0 = Tidak Diabetes, 1 = Diabetes).

## Output Analisis

- **PCA Output**:
  - Proporsi varians untuk setiap komponen utama.
  - Matriks *eigenvectors*.
  - Grafik *scree plot*, *biplot*, dan *correlation circle*.

- **FA Output**:
  - Faktor utama dengan *loadings* masing-masing variabel.
  - Diagram faktor untuk memvisualisasikan hubungan antar variabel.

## Teknologi yang Digunakan

- **R**: Bahasa pemrograman utama untuk analisis data.
- **psych**: Untuk analisis faktor dan KMO test.
- **FactoMineR** dan **factoextra**: Untuk analisis dan visualisasi PCA.
- **ggplot2** dan **gridExtra**: Untuk keperluan visualisasi data.

## Catatan Penting

- Pastikan file dataset `diabetes.csv` berada dalam direktori yang sama dengan skrip R.
- Pastikan semua pustaka R yang diperlukan telah diinstal sebelum menjalankan analisis.

## Kontribusi

Kontribusi sangat dihargai! Silakan buat pull request atau ajukan *issue* jika Anda memiliki ide atau menemukan bug.

## Lisensi

Proyek ini dilisensikan di bawah [MIT License](LICENSE).

