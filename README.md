# Big Data Analytics UMKM Coto HB'Eng
Proyek ini menganalisis data transaksi bisnis UMKM Coto HBeng untuk memberikan wawasan dan prediksi menggunakan berbagai teknik machine learning. Tujuannya adalah untuk mengoptimalkan strategi operasional dan proses pengambilan keputusan bisnis.

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Data Preprocessing](#data-preprocessing)
4. [Machine Learning Algorithms](#machine-learning-algorithms)
5. [Results and Discussion](#results-and-discussion)
6. [Conclusion](#conclusion)
7. [References](#references)
---

## Introduction

Analisis data ini dilakukan dengan tujuan meningkatkan penjualan, dimana dengan mengetahui produk atau menu mana yang paling laris, maka pemilik bisa memprioritaskan stok bahan baku untuk menu tersebut. Selain itu, ini juga dapat meningkatkan efisiensi operasional karena pemilik warung dapat mengetahui waktu yang ramai sehingga pengaturan shift karyawan dapat dioptimalkan.

---

## Dataset

Dataset berisi data transaksi harian yang mencakup informasi berikut:
- **Tanggal**: Tanggal transaksi.
- **Waktu**: Waktu transaksi.
- **Menu**: Nama menu yang dipesan.
- **Harga**: Harga per unit menu (dalam Rupiah).
- **Jumlah**: Jumlah pesanan.
- **Total**: Total harga transaksi (dalam Rupiah).

---

## Data Preprocessing

Tahapan preprocessing yang dilakukan meliputi:

1. **Data Integration**:
   - Menggabungkan dataset transaksi.
   - Mengecek format dan isi data.

2. **Data Reduction**:
   - Menghapus data duplikat.
   - Mengisi atau menghapus data yang kosong.

3. **Data Transformation**:
   - Mengonversi format kolom, seperti `Tanggal` ke `datetime` dan `Harga` ke format numerik.
   - Menambahkan fitur baru:
     - **Nama Hari** (misalnya: Senin, Selasa).
     - **Kategori Waktu** (Pagi, Siang, Malam).

---

## Machine Learning Algorithms

Tiga algoritma machine learning digunakan untuk menganalisis data dan membuat prediksi:

1. **Linear Regression**  
   Model sederhana untuk memprediksi tren penjualan berdasarkan waktu.

2. **Random Forest**  
   Model berbasis pohon keputusan untuk menangani pola data yang lebih kompleks.

3. **Apriori Algorithm**  
   Algoritma digunakan untuk menganalisis kombinasi menu yang paling sering dibeli bersamaan dalam satu hari.

---

## Results and Discussion

1. **Daily Menu Analysis**  
   Analisis ini bertujuan untuk mengetahui menu yang paling sering dipesan setiap harinya. Hasil ini membantu dalam menentukan prioritas stok bahan baku untuk menu favorit pelanggan.

2. **Predict Future Sales**  
   Dengan menggunakan algoritma machine learning seperti *Linear Regression* dan *Random Forest*, analisis ini memprediksi jumlah penjualan di masa depan. Informasi ini bermanfaat untuk memperkirakan kebutuhan bahan baku dan strategi promosi.

3. **Peak Hour Analysis**  
   Analisis ini mengidentifikasi jam-jam sibuk dalam sehari ketika transaksi paling banyak terjadi. Temuan ini dapat digunakan untuk mengatur shift karyawan agar operasional berjalan lebih efisien.

4. **Identifying Frequent Menu Set**  
   Dengan algoritma *Apriori*, analisis ini menemukan kombinasi menu yang sering dipesan bersama dalam satu transaksi. Hasil ini dapat membantu dalam membuat paket promosi atau menu combo yang menarik bagi pelanggan.

5. **Total Daily Sales**  
   Analisis ini menghitung total penjualan harian untuk memantau performa bisnis secara keseluruhan. Dengan informasi ini, pemilik usaha dapat mengevaluasi tren pendapatan dan menentukan target penjualan di masa depan.

---

## Conclusion

Analisis data penjualan UMKM Coto HBeng menunjukkan bahwa identifikasi menu favorit harian dapat membantu prioritas stok bahan baku, sementara prediksi penjualan masa depan dengan algoritma *Linear Regression* dan *Random Forest* memberikan wawasan untuk perencanaan strategis. Jam-jam sibuk yang teridentifikasi memungkinkan pengaturan shift karyawan secara efisien, sedangkan analisis kombinasi menu dengan algoritma *Apriori* membuka peluang untuk merancang paket promosi yang menarik. Selain itu, pemantauan total penjualan harian memungkinkan evaluasi performa bisnis secara real-time. Secara keseluruhan, hasil analisis ini memberikan dasar yang kuat untuk mengoptimalkan strategi operasional, meningkatkan kepuasan pelanggan, dan mendukung pertumbuhan bisnis UMKM Coto HBeng secara berkelanjutan.

---

## References
 1. https://scikit-learn.org/stable/modules/linear_model.html#ordinary-least-squares
 2. https://scikit-learn.org/stable/modules/ensemble.html#random-forests 
 3. https://rasbt.github.io/mlxtend/user_guide/frequent_patterns/apriori/
 4. https://matplotlib.org/stable/users/index.html
