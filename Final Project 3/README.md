Python for Data Science - MSIB Batch 4 

Kelompok 3

1. M. Haikal Febrian
2. Naurah Nadzifah Azizi
3. Nadia Syachrani
4. Muhammad Randy

PYTN-KS11

**FINAL PROJECT 3**

# Latar Belakang
Penyakit kardiovaskular (CVD) adalah penyebab kematian nomor 1 di seluruh dunia, yang diperkirakan menewaskan 17,9 juta orang setiap tahunnya, yang merupakan 31% dari seluruh kematian di seluruh dunia.
Gagal jantung adalah kejadian umum yang disebabkan oleh CVD dan kumpulan data ini berisi 12 fitur yang dapat digunakan untuk memprediksi kematian akibat gagal jantung.

Sebagian besar penyakit kardiovaskular dapat dicegah dengan mengatasi faktor risiko perilaku seperti penggunaan tembakau, pola makan yang tidak sehat dan obesitas, kurangnya aktivitas fisik, dan penggunaan alkohol yang berbahaya dengan menggunakan strategi yang berlaku di seluruh populasi.

Orang dengan penyakit kardiovaskular atau yang memiliki risiko kardiovaskular tinggi (karena adanya satu atau lebih faktor risiko seperti hipertensi, diabetes, hiperlipidemia, atau penyakit yang sudah ada sebelumnya) memerlukan deteksi dini dan manajemen di mana model pembelajaran mesin dapat sangat membantu.

# Objektif:
Tujuannya adalah untuk mengidentifikasi faktor-faktor yang memiliki pengaruh signifikan dalam memprediksi kemungkinan kematian akibat gagal jantung dan memprediksi kemungkinan terjadinya kematian dengan mempertimbangkan faktor-faktor tersebut menggunakan metode ensemble

# Data:
Untuk proyek ini kami mengambil dataset dari kaggle di mana terdapat 299 baris dan 13 kolom dan file tersebut dalam format csv. Anda dapat melihat atau mengunduh dataset melalui tautan ini: https://www.kaggle.com/andrewmvd/heart-failure-clinical-data

# Penerapan Proyek ini:
Kami menggunakan algoritma pembelajaran mesin dengan model ensemble yaitu random forest dan gradient boosting untuk kemungkinan kematian akibat gagal jantung, sehingga mudah untuk melakukan analisis terjadinya kematian berdasarkan fitur tertentu. Atribut yang menjadi target yaitu atribut Death Event/Kematian, sedangkan atribut lainnya merupakan prediktor.

# Kesimpulan
## Kesimpulan terhadap EDA :
* Terdapat 192 data pasien dengan rata-rata usia sebesar 60 tahun, rentang usia antara 40 hingga 95 tahun
* Terdapat 103 pasien yang tidak menderita anemia.
* Terdapat 106 pasien yang tidak menderita diabetes.
* Terdapat 127 pasien yang tidak menderita tekanan darah tinggi.
* Terdapat 119 pasien laki-laki
* Terdapat 138 pasien yang tidak merokok.
* Terdapat 96 pasien yang tidak meninggal.

Dalam kelompok yang tidak merokok, persentase kematian adalah sekitar 47% (66 dari total 138 pasien tidak merokok). Sedangkan dalam kelompok yang merokok, persentase kematian adalah sekitar 55% (30 dari total 54 pasien merokok). Hal ini menunjukkan bahwa tingkat kematian cenderung lebih tinggi pada pasien yang merokok. Oleh karena itu, merokok dapat menjadi faktor risiko dalam kejadian kematian pada pasien dengan gagal jantung.

## Kesimpulan terhadap Model :
* Dapat disimpulkan bahwa model Decision Tree dan Random Forest memiliki performa yang serupa dalam hal akurasi, namun Decision Tree memiliki nilai presisi yang sedikit lebih tinggi. Model Gradient Boosting memiliki performa yang sedikit lebih tinggi daripada model Decision Tree dan Random Forest dalam hal akurasi, racll, dan F1 Score. 
* Akurasi RF dan DT : 0.7692 lebih kecil dibandingkan Akurasi GB : 0.7949
* Akurasi ketiga model tersebut berada pada nilai > 70%, sehingga untuk memprediksi kemungkinan terjadinya kematian akibat gagal jantung bisa menggunakan Random Forest, Decision Tree atau Gradient Boosting tergantung kebutuhan, karena keduanya menghasilkan tingkat akurasi model yang nilainya hampir sama
* Pada kasus ini, performa model Random Forest, Decisiion Tree, dan Gradient Boosting cukup seimbang antara data train dan test dengan perbedaan skor yang tidak terlalu jauh. Oleh karena itu, dapat dikatakan bahwa model ini tidak mengalami overfitting atau underfitting.
* Skor akurasi, presisi, recall dan f1 score model Random Forest, Decisiion Tree, dan Gradient Boosting sudah cukup baik (> 0.7)
