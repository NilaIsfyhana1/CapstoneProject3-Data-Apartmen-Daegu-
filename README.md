# Prediksi Harga Apartemen di Daegu

## Latar Belakang Masalah
Daegu, kota terbesar ketiga di Korea Selatan, menghadapi tantangan dalam pasar properti akibat penentuan harga apartemen yang subjektif oleh pemilik. Dengan lebih dari 240.000 unit apartemen pada tahun 2021, sebagian besar transaksi dilakukan melalui agen properti. Namun, praktik penentuan harga yang kurang efisien menyebabkan waktu penjualan yang lama atau potensi keuntungan yang hilang. Proyek ini bertujuan untuk mengatasi masalah ini dengan menggunakan machine learning untuk memprediksi harga apartemen berdasarkan faktor internal dan eksternal.

## Permasalahan
Proses penjualan apartemen di Daegu menghadapi masalah berikut:
- Harga terlalu tinggi sehingga unit sulit terjual.
- Harga terlalu rendah sehingga pemilik kehilangan potensi keuntungan.

Model berbasis data diperlukan untuk:
1. Menentukan harga yang akurat sesuai kondisi pasar.
2. Mengidentifikasi faktor utama yang memengaruhi harga apartemen.

## Tujuan
- **Mengembangkan Model Prediksi Harga:** Membuat model machine learning untuk memprediksi harga apartemen berdasarkan variabel seperti ukuran, lokasi, fasilitas, dan jarak ke transportasi umum.
- **Analisis Faktor Penting:** Mengidentifikasi variabel yang paling memengaruhi harga apartemen.
- **Evaluasi Model:** Memvalidasi akurasi model menggunakan metrik seperti MAE, RMSE, dan R².

## Pendekatan Analisis
1. **Eksplorasi Data:** Menganalisis hubungan antara fitur (misalnya jarak ke stasiun, luas apartemen) dengan harga.
2. **Modeling:** Melatih dan mengevaluasi beberapa algoritma:
   - Linear Regression
   - K-Nearest Neighbors (KNN)
   - Decision Tree
   - Random Forest
   - XGBoost
   Melakukan tuning hyperparameter untuk kinerja optimal.
3. **Analisis Faktor Penting:** Menggunakan model seperti Random Forest dan XGBoost untuk menentukan faktor utama yang memengaruhi harga.
4. **Evaluasi:** Membandingkan performa model menggunakan MAE, RMSE, dan R² untuk memilih model terbaik.

## Hasil
- **Model Terbaik:** XGBoost memberikan performa terbaik:
  - Sebelum tuning: RMSE = 46,401.53, MAE = 37,852.76
  - Setelah tuning: RMSE = 46,261.44, MAE = 37,723.99
  
- **Fitur Utama:**
  - Tipe apartemen (terraced)
  - Ukuran apartemen
  - Jumlah tempat parkir basement

Model XGBoost mengurangi kesalahan prediksi sebesar 68,4% (₩82,158) dibandingkan model berbasis aturan, memungkinkan rekomendasi harga yang lebih akurat dan proses penjualan yang lebih cepat.

## Rekomendasi
### Peningkatan Model
1. Tambahkan fitur relevan (misalnya, lantai apartemen, jumlah kamar tidur, indeks harga konsumen, PDB).
2. Tingkatkan kualitas dan jumlah data dengan menyertakan data historis dan tren pasar.
3. Jelajahi model lanjutan (misalnya, RNN) untuk analisis tren waktu.

### Rekomendasi Bisnis
1. Fokuskan pemasaran pada apartemen tipe terraced dan unit berukuran besar.
2. Tonjolkan fasilitas seperti parkir basement dan fitur keamanan.
3. Prioritaskan properti dekat transportasi umum dan fasilitas umum.
4. Integrasikan tren pasar dan kondisi ekonomi dalam strategi penentuan harga.

## Kesimpulan
Proyek ini menunjukkan pentingnya machine learning dalam mengoptimalkan penentuan harga apartemen di Daegu. Dengan wawasan berbasis data, agen properti dapat meningkatkan efisiensi penjualan dan memaksimalkan keuntungan bagi pemilik properti.
