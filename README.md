# Klasifikasi-Tingkat-Kemiskinan-di-Indonesia-Menggunakan-Agoritma-KNN

## 📌 Deskripsi Proyek
Proyek ini bertujuan untuk menganalisis dan mengklasifikasikan tingkat kemiskinan di Indonesia berdasarkan berbagai indikator sosial dan ekonomi menggunakan algoritma **K-Nearest Neighbors (KNN)**. Dengan memanfaatkan dataset yang berisi informasi terkait tingkat kemiskinan, indeks pembangunan manusia (IPM), pengeluaran per kapita, serta faktor lainnya, model ini dapat memberikan wawasan tentang faktor-faktor yang memengaruhi tingkat kemiskinan.

## 🗂 Dataset
Dataset yang digunakan dalam proyek ini berasal dari **Klasifikasi Tingkat Kemiskinan di Indonesia.csv**. Data ini berisi berbagai indikator ekonomi dan sosial dari berbagai kabupaten/kota di Indonesia.

Beberapa fitur yang digunakan dalam analisis ini antara lain:
- **P0_Persen**: Persentase penduduk miskin di suatu daerah.
- **Rata_rata_Lama_Sekolah**: Rata-rata lama sekolah penduduk berusia 15 tahun ke atas.
- **Pengeluaran_per_Kapita**: Pengeluaran per kapita dalam ribu rupiah per orang per tahun.
- **IPM**: Indeks Pembangunan Manusia.
- **Umur_Harapan_Hidup**: Perkiraan usia harapan hidup.
- **Akses_Sanitasi_Layak**: Persentase rumah tangga dengan akses terhadap sanitasi layak.
- **Akses_Air_Minim_Layak**: Persentase rumah tangga dengan akses terhadap air minum layak.
- **Pengangguran_Terbuka**: Tingkat pengangguran terbuka.
- **Partisipasi_Angkatan_Kerja**: Tingkat partisipasi angkatan kerja.
- **PDRB_Harga_Konstan**: Produk Domestik Regional Bruto berdasarkan harga konstan.

## 📌 Instalasi dan Persiapan
Pastikan Anda telah menginstal Python dan pustaka yang diperlukan sebelum menjalankan proyek ini. Anda dapat menginstalnya dengan perintah berikut:

## 📊 Tahapan Analisis
1. **Membaca dan membersihkan data**  
   - Mengganti nama kolom agar lebih mudah digunakan.
   - Mengonversi angka desimal yang berbentuk string menjadi tipe data numerik.
   - Menghapus data yang mengandung nilai kosong.

2. **Preprocessing Data**  
   - Menentukan fitur (X) dan target (y).
   - Melakukan standarisasi fitur menggunakan **StandardScaler**.
   - Membagi dataset menjadi **data latih (train)** dan **data uji (test)** dengan rasio **80:20**.

3. **Membangun Model K-Nearest Neighbors (KNN)**  
   - Menggunakan **KNeighborsClassifier** dengan **k=5**.
   - Melatih model dengan data latih.
   - Memprediksi klasifikasi tingkat kemiskinan pada data uji.
   - Mengevaluasi performa model menggunakan **classification_report** dan **accuracy_score**.

4. **Visualisasi Data**  
   - **Scatter plot** untuk melihat hubungan antara persentase penduduk miskin dan IPM.
   - **Histogram** distribusi IPM.
   - **Heatmap korelasi** antar variabel.
   - **Scatter plot** hubungan antara pengeluaran per kapita dan tingkat kemiskinan.

## 📈 Hasil dan Evaluasi
- Model **KNN** mampu mengklasifikasikan tingkat kemiskinan dengan tingkat akurasi tertentu.
- Visualisasi data menunjukkan hubungan yang jelas antara faktor-faktor sosial dan ekonomi dengan tingkat kemiskinan.
- Hasil analisis ini dapat digunakan untuk mendukung pengambilan keputusan dalam kebijakan sosial-ekonomi serta memberikan wawasan tentang faktor-faktor yang memengaruhi kemiskinan di Indonesia.

## 📌 Cara Menjalankan Kode
1. Clone repositori ini:
   ```bash
   git clone https://github.com/username/repo-name.git
   cd repo-name
   ```
2. Jalankan script Python:
   ```bash
   python script.py
   ```

## 📚 Teknologi yang Digunakan
- **Python**
- **Pandas** untuk manipulasi data
- **NumPy** untuk operasi numerik
- **Matplotlib & Seaborn** untuk visualisasi data
- **Scikit-learn** untuk pemodelan machine learning

## 🙌 Kontribusi dan Pengembangan
Jika Anda ingin berkontribusi atau mengembangkan proyek ini lebih lanjut, silakan lakukan **fork** dan ajukan **pull request** dengan peningkatan atau analisis tambahan.

## 🎯 Kesimpulan
Proyek ini menunjukkan bagaimana **machine learning**, khususnya algoritma **KNN**, dapat digunakan untuk memahami faktor-faktor kemiskinan di Indonesia. Dengan model ini, kita dapat mengidentifikasi pola dan memberikan wawasan berbasis data untuk membantu dalam pengambilan keputusan terkait kebijakan sosial dan ekonomi.
