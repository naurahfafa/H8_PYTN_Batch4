Python for Data Science - MSIB Batch 4 

Kelompok 3

1. M. Haikal Febrian
2. Naurah Nadzifah Azizi
3. Nadia Syachrani
4. Muhammad Randy

PYTN-KS11

**FINAL PROJECT 2**

# Objektif:
Tujuannya adalah untuk mengidentifikasi faktor-faktor yang memiliki pengaruh signifikan terhadap kemungkinan terjadinya hujan dan untuk memprediksi kemungkinan terjadinya hujan pada suatu tempat berdasarkan faktor-faktor cuaca yang mempengaruhinya menggunakan dua metode, yaitu Logistic Regression dan Support Vector Machine.

# Data:
Untuk proyek ini kami mengambil dataset dari kaggle di mana terdapat 145460 baris dan 23 kolom dan file tersebut dalam format csv. Anda dapat melihat atau mengunduh dataset melalui tautan ini: https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package

# Penerapan Proyek ini:
Kami menggunakan algoritma pembelajaran mesin dengan model logistik regresi dan support vector machine untuk memprediksi besok hujan, sehingga mudah untuk melakukan analisis terjadinya hujan berdasarkan fitur tertentu.

# Kesimpulan
## Kesimpulan terhadap EDA :
* Portland merupakan kota di wilayah Pasifik Barat laut Amerika Serikat yang memiliki curah hujan yang paling tinggi. Beberapa faktor yang menyebabkan hal ini antara lain letak geografis yang berhadapan langsung dengan Samudra Pasifik, medan pegunungan yang dapat mempengaruhi pola aliran udara, serta pola aliran udara yang mengarah ke wilayah pesisir barat laut Amerika Serikat selama musim dingin.
* Frekuensi angin dari arah barat di Australia mungkin tinggi karena wilayah tersebut memiliki relief topografi yang beragam dan terletak dekat garis khatulistiwa. Sedangkan frekuensi angin dari arah timur tenggara rendah karena wilayah tersebut tidak memiliki kecenderungan angin dari arah itu.
* Distribusi curah hujan relatif seragam di seluruh lokasi, namun terdapat beberapa lokasi yang memiliki curah hujan yang lebih rendah dibandingkan dengan lokasi lainnya. Beberapa lokasi yang terlihat memiliki curah hujan yang lebih rendah antara lain  Nhil, Katherine, dan Uluru. Sedangkan Portland menerima curah hujan paling banyak di antara 49 lokasi yang tersedia dalam dataset.
* Semakin banyak awan pada pukul 3 sore, semakin tinggi kemungkinan turun hujan besok. Ketika jumlah awan mencapai 6, kemungkinan turun hujan besok mencapai puncaknya. Sedangkan ketika jumlah awan semakin sedikit, kemungkinan hujan besok cenderung rendah. Hal ini mungkin disebabkan oleh fakta bahwa awan adalah indikator utama cuaca hujan, dan semakin banyak awan, semakin besar kemungkinan terjadi hujan.
* Dapat dilihat bahwa ketika hari ini turun hujan, kemungkinan besok juga turun hujan lebih tinggi dibandingkan ketika hari ini tidak turun hujan. 

## Kesimpulan terhadap Model :
* Berdasarkan Metrics Performence untuk Logistic Regression dan Support Vector Machine model, keduanya memberikan nilai yang sangat bagus serta kedua model tersebut memiliki akurasi yang tidak jauh berbeda. 
* Akurasi LR : 0.7083 lebih besar dibandingkan Akurasi SVM : 0.7091
* Akurasi kedua model tersebut berada pada nilai 70%, sehingga untuk memprediksi kejadian hujan untuk selanjutnya bisa menggunakan SVM atau Logistic Regression tergantung kebutuhan, karena keduanya menghasilkan tingkat akurasi model yang nilainya hampir sama
* Pada kasus ini, performa model LR dan SVM cukup seimbang antara data train dan test dengan perbedaan skor yang tidak terlalu jauh. Oleh karena itu, dapat dikatakan bahwa model ini tidak mengalami overfitting atau underfitting.
* Skor akurasi, presisi, recall dan f1 score pada kedua model sudah cukup baik (> 0.7).
