Python for Data Science - MSIB Batch 4 

Kelompok 3

1. M. Haikal Febrian
2. Naurah Nadzifah Azizi
3. Nadia Syachrani
4. Muhammad Randy

PYTN-KS11

**FINAL PROJECT 4 - CREDIT CARD DATASET FOR CLUSTERING**

# Latar Belakang
Penggunaan kartu kredit telah menjadi metode pembayaran yang umum digunakan di era digital saat ini.  Bagi perusahaan kartu kredit dan lembaga keuangan, memahami pola penggunaan kartu kredit oleh pelanggan mereka sangat penting. Itu membantu mereka dalam mengidentifikasi kebiasaan pengeluaran, perilaku pembayaran, dan pola penggunaan yang dapat membantu mereka dalam mengambil keputusan bisnis yang lebih baik.

Dengan memanfaatkan dataset ini, perusahaan kartu kredit dan lembaga keuangan dapat meningkatkan pemahaman tentang perilaku pengguna kartu kredit, mengoptimalkan strategi bisnis, dan meningkatkan kepuasan pelanggan.

# Objektif:
Tujuannya adalah untuk memahami konsep clustering dengan menggunakan Scikit-Learn, mempersiapkan data untuk digunakan dalam Clustering, dan  mengimplementasikan clustering pada data credit card.

# Data:
Untuk proyek ini kami mengambil dataset dari kaggle di mana terdapat 8950 baris dan 18 kolom dan file tersebut dalam format csv. Anda dapat melihat atau mengunduh dataset melalui tautan ini: https://www.kaggle.com/datasets/arjunbhasin2013/ccdata

# Penerapan Proyek ini:
Kami menggunakan algoritma pembelajaran mesin dengan model clustering untuk mengelompokkan data ke dalam kelompok-kelompok yang memiliki kesamaan berdasarkan pola atau karakteristik yang ada dalam data tersebut.

# Kesimpulan
## Kesimpulan terhadap EDA :
* Terdapat 18 atribut yang menjadi kriteria masing-masing customer yang kemudian dipilih 12 atribut yang saling independen (dilihat dari korelasi) untuk pembentukan klaster.
* Berdasarkan jumlah frekuensi, cluster 2 memiliki frekuensi yang paling tinggi daripada cluster 0, 1, dan 3, sedangkan cluster 3 memiliki frekuensi paling rendah diantara cluster lainnya.
* Pola Pengeluaran: Jumlah pembelian secara keseluruhan cenderung tinggi (rata-rata 1.38) di semua kluster. Pembelian dengan satu kali transaksi (one-off purchases) cenderung rendah (rata-rata 0.41). Pembelian dengan angsuran (installments purchases) cenderung rendah (rata-rata 0.19).
* Pola Pembayaran: Jumlah pembayaran cenderung tinggi (rata-rata 0.54) di semua kluster. Pembayaran minimum cenderung tinggi (rata-rata 0.63) di semua kluster. Persentase pembayaran penuh (PRC_FULL_PAYMENT) cenderung rendah (rata-rata 0.22) di semua kluster.
* Saldo Kartu: Saldo kartu cenderung positif (rata-rata 0.28) di semua kluster, menunjukkan kecenderungan penggunaan kartu kredit.
* Penggunaan Kemajuan Tunai: Penggunaan kemajuan tunai (cash advance) cenderung rendah (rata-rata 0.44) di semua kluster. Jumlah transaksi kemajuan tunai (cash advance trx) juga cenderung rendah (rata-rata 0.47) di semua kluster.

## Kesimpulan terhadap Model :
* Cluster digunakan untuk memisahkan kelompok-kelompok data yang berbeda. Berdasarkan hasil diatas, algoritma sudah baik dalam memisahkan kelompok-kelomppoknya, tetapi didalam cluster masih sedikit tercampur dengan cluster lain. Kita dapat melihat beberapa jenis cluster yang berbeda, diantaranya cluster 0, 1, 2, dan 3. Kita mungkin melihat outliers dari beberapa data tersebut.
* Setiap kolom memiliki jumlah data yang sama, yaitu 1864 untuk Klaster 0, 2360 untuk Klaster 1, 2915 untuk Klaster 2, dan 1811 untuk Klaster 3..
* Kluster 0: Saldo tinggi, pembelian dan transaksi tinggi, batas kredit tinggi, pembayaran tinggi.
* Kluster 1: Saldo rendah, pembelian dan transaksi rendah, batas kredit rendah, pembayaran rendah.
* Kluster 2: Saldo sedang, pembelian dan transaksi sedang, batas kredit sedang, pembayaran rendah.
* Kluster 3: Saldo rendah, pembelian dan transaksi rendah, batas kredit rendah, pembayaran tinggi.
* Dalam ringkasan, kluster 0 menunjukkan kebiasaan pengguna yang baik dalam mengelola keuangan, sedangkan kluster 1 menunjukkan kebiasaan yang buruk. Kluster 2 menunjukkan kebiasaan yang sedang, sementara kluster 3 menunjukkan kombinasi saldo rendah dengan pembayaran yang baik.
