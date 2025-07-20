# Analisis Kesejahteraan Provinsi di Indonesia 

Proyek ini bertujuan untuk melakukan analisis pengelompokan (clustering) provinsi-provinsi di Indonesia berdasarkan berbagai indikator kesejahteraan menggunakan algoritma **K-Means**.

---

## Daftar Isi

1.  [Latar Belakang](#latar-belakang)
2.  [Tujuan Proyek](#tujuan-proyek)
3.  [Dataset](#dataset)
4.  [Metodologi](#metodologi)
5.  [Hasil Clustering](#hasil-clustering)
6.  [Tech Stack](#tech-stack)
7.  [Cara Menjalankan Proyek](#cara-menjalankan-proyek)

---

## Latar Belakang

Tingkat kesejahteraan di setiap provinsi di Indonesia sangat bervariasi. Memahami pengelompokan provinsi berdasarkan indikator-indikator kunci seperti Harapan Hidup, Pengeluaran, dan Rata-rata Lama Sekolah sangat penting bagi pemerintah dan pemangku kebijakan untuk merancang program pembangunan yang tepat sasaran dan merata.

## Tujuan Proyek

-   Mengidentifikasi kelompok (cluster) provinsi dengan karakteristik kesejahteraan yang serupa.
-   Menganalisis ciri-ciri utama dari setiap cluster yang terbentuk.
-   Menyediakan wawasan berbasis data mengenai peta kesejahteraan di Indonesia.

---

## Dataset

Dataset yang digunakan dalam analisis ini mencakup beberapa indikator kunci kesejahteraan untuk setiap provinsi di Indonesia, antara lain:
-   **Harapan Hidup**: Angka harapan hidup saat lahir.
-   **Pengeluaran**: Rata-rata pengeluaran per kapita.
-   **Rata-rata Lama Sekolah**: Rata-rata jumlah tahun pendidikan yang ditempuh oleh penduduk.

---

## Metodologi

Analisis ini menggunakan algoritma **K-Means Clustering**, sebuah metode *unsupervised learning* untuk mengelompokkan data ke dalam sejumlah *k* cluster. Langkah-langkah utamanya meliputi:
1.  **Pengumpulan Data**: Mengumpulkan data indikator kesejahteraan per provinsi.
2.  **Pra-pemrosesan**: Membersihkan dan melakukan standarisasi (scaling) pada data agar setiap fitur memiliki skala yang sebanding.
3.  **Pemodelan**: Menerapkan algoritma K-Means untuk mengelompokkan provinsi ke dalam 3 cluster.
4.  **Analisis Cluster**: Menganalisis karakteristik rata-rata dari setiap cluster untuk memahami profilnya.

---

## Hasil Clustering

Berdasarkan analisis K-Means, provinsi-provinsi di Indonesia berhasil dikelompokkan ke dalam **3 cluster** dengan profil sebagai berikut:

-   **Cluster 0: Kesejahteraan Rendah**
    -   Terdiri dari **11 provinsi**.
    -   **Karakteristik**: Memiliki nilai rata-rata **Harapan Hidup**, **Pengeluaran**, dan **Rata-rata Lama Sekolah** yang paling rendah dibandingkan cluster lainnya.
    -   **Contoh Provinsi**: Papua, Nusa Tenggara Timur.

-   **Cluster 1: Kesejahteraan Tinggi**
    -   Terdiri dari **9 provinsi**.
    -   **Karakteristik**: Memiliki nilai rata-rata **Harapan Hidup**, **Pengeluaran**, dan **Rata-rata Lama Sekolah** yang paling tinggi.
    -   **Contoh Provinsi**: DKI Jakarta, DI Yogyakarta.

-   **Cluster 2: Kesejahteraan Sedang**
    -   Terdiri dari **14 provinsi**.
    -   **Karakteristik**: Nilai rata-rata untuk ketiga indikator berada di antara Cluster 0 dan Cluster 1.
    -   **Contoh Provinsi**: Jawa Barat, Jawa Tengah.

---

## Tech Stack

-   **Bahasa Pemrograman**: Python
-   **Library Analisis**: Pandas, NumPy
-   **Library Machine Learning**: Scikit-learn
-   **Library Visualisasi**: Matplotlib, Seaborn

---

## Cara Menjalankan Proyek

1.  **Clone Repositori Ini**
    ```bash
    git clone https://github.com/haaahabib/analisis-kesejahteraan.git
    ```
2.  **Masuk ke Direktori Proyek**
    ```bash
    cd analisis-kesejahteraan
    ```
3.  **Install Library yang Dibutuhkan**
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn jupyter
    ```
4.  **Jalankan Jupyter Notebook**
    Buka dan jalankan file `main.ipynb` untuk melihat seluruh proses analisis dan visualisasi.
    ```bash
    jupyter notebook main.ipynb
    ```
