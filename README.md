# Laporan Proyek DMML
A. Afif Alhaq - H071221064
Adrian Hidayat - H071221091
Evan Pandu - H071221057

## Domain Proyek

Stroke merupakan suatu kondisi kesehatan serius yang terjadi ketika pasokan darah ke bagian otak terganggu atau terputus, menyebabkan sel-sel otak tidak mendapatkan cukup oksigen dan nutrisi. Kondisi ini dapat berdampak fatal dan memiliki dampak yang signifikan pada kesehatan seseorang. Menurut Data pada artikel [2], stroke menjadi penyebab utama kematian di Indonesia. Bahkan prevalensi pasien stroke meningkat dari 7% per mil menjadi 10,9% per mil [3]. Statistik ini mencerminkan urgensi untuk mengembangkan model machine learning yang dapat memprediksi risiko stroke pada individu, sebagai langkah proaktif dalam mengurangi beban kesehatan global yang disebabkan oleh stroke.

Pentingnya memprediksi risiko stroke juga dapat dilihat dari data-data konkret. Misalnya, dalam konteks internasional, Stroke menyerang sekitar 15 juta orang per tahun [4], dan dampaknya tidak hanya terbatas pada tingkat kematian. Banyak yang selamat dari stroke mengalami kecacatan jangka panjang, memerlukan perawatan intensif, dan mengalami penurunan kualitas hidup yang signifikan. Oleh karena itu, upaya preventif menjadi krusial untuk mengurangi beban sosial dan ekonomi yang ditimbulkan oleh stroke.

Dalam upaya meningkatkan pemahaman dan pencegahan terhadap stroke, sebuah proyek penelitian akan dilakukan untuk mengembangkan model machine learning yang dapat memprediksi risiko stroke pada individu. Proyek ini akan melibatkan analisis berbagai faktor kesehatan, seperti tekanan darah, kadar gula darah, indeks massa tubuh (BMI), riwayat merokok, dan faktor risiko lainnya yang dapat mempengaruhi kemungkinan seseorang mengalami stroke. Dimana variabel-variabel tersebut didukung oleh data, yang mengatakan bahwa penyebab stroke dapat diakibatkan oleh tekanan darah, kurangnya aktivitas fisik, konsumsi makanan, kebiasaan merokok, dan faktor-faktor lainnya [3].

Dengan memanfaatkan data kesehatan dan riwayat medis, model ini diharapkan dapat memberikan prediksi akurat tentang risiko stroke pada seseorang. Implementasi proyek ini dapat membantu para profesional medis dalam memberikan peringatan dini kepada pasien dengan risiko tinggi, sehingga tindakan pencegahan dapat diambil lebih awal. Selain itu, model ini dapat menjadi alat yang berguna bagi masyarakat dalam memahami dan mengelola faktor risiko kesehatan mereka, serta mendukung kebijakan kesehatan masyarakat yang lebih proaktif dalam pencegahan stroke.

## Business Understanding

Proyek ini dibangun untuk membantu para profesional medis dalam memberikan peringatan dini kepada pasien dengan risiko tinggi, sehingga tindakan pencegahan dapat diambil lebih awal. Selain itu, model ini dapat menjadi alat yang berguna bagi masyarakat dalam memahami dan mengelola faktor risiko kesehatan mereka, serta mendukung kebijakan kesehatan masyarakat yang lebih proaktif dalam pencegahan stroke.

### Problem Statements

- Bagaimana mengidentifikasi faktor-faktor risiko yang berkontribusi pada kemungkinan seseorang terkena stroke?
- Bagaimana membangun model prediktif untuk memprediksi risiko seseorang terkena stroke berdasarkan faktor-faktor tertentu?
- Bagaimana menentukan dampak variabel-variabel tertentu terhadap prediksi risiko stroke?

### Goals

- Menganalisis faktor-faktor risiko yang berkontribusi pada kemungkinan seseorang terkena stroke.
- Mengembangkan model machine learning untuk memprediksi risiko stroke berdasarkan variabel-variabel tertentu.
- Menyajikan hasil analisis dan model secara jelas dan terukur untuk mendukung pengambilan keputusan.

Kriteria/Ukuran Hasil Analisis yang Terukur:
- Menyajikan temuan analisis dengan tingkat kejelasan yang tinggi, disertai dengan visualisasi yang mendukung.
- Model machine learning memiliki tingkat akurasi dan kehandalan yang dapat diukur.

Metrik Khusus untuk Evaluasi Keberhasilan:
- Akurasi model prediktif sebagai indikator seberapa baik model dapat memprediksi kasus positif dan negatif.
- Presisi sebagai metrik untuk mengukur seberapa banyak prediksi positif yang benar-benar relevan.
- Recall untuk menilai kemampuan model mengidentifikasi sebanyak mungkin kasus positif.
- F1-score sebagai keseimbangan antara presisi dan recall.

### Solution statements
- Menyiapkan data agar dapat digunakan untuk proses analisis dan pemodelan machine learning.
- Melakukan eksplorasi data untuk memahami hubungan antar variabel dan melihat tren dalam dataset.
- Melakukan feature engineering (Standarisasi, *One-hot-encoding*) untuk meningkatkan kinerja model.
- Membangun model prediktif menggunakan algoritma klasifikasi seperti *K-Nearest Neighbors*, *Random Forest* dan *Adaptive Boosting*.
- Melakukan evaluasi model menggunakan metrik evaluasi yang relevan seperti akurasi, presisi, *recall*, dan *F1-score*. Memilih model terbaik berdasarkan performa evaluasi.
- Melakukan *hyperparameter tuning* menggunakan *grid search* untuk meningkatkan performa model.

Kontribusi Model dalam Kesehatan Masyarakat:
- Penyadaran Risiko Stroke: Model ini dapat memberikan informasi kepada masyarakat tentang faktor risiko stroke yang perlu diwaspadai. Dengan pemahaman ini, individu dapat mengambil langkah-langkah preventif yang lebih baik.
- Pengelolaan Faktor Risiko Kesehatan: Melalui hasil prediksi model, masyarakat dapat mengelola faktor risiko kesehatan mereka secara lebih efektif. Misalnya, dengan menyesuaikan pola makan, meningkatkan aktivitas fisik, atau mengontrol tekanan darah, mereka dapat mengurangi risiko stroke.
- Dukungan Kebijakan Kesehatan Masyarakat: Model ini dapat menjadi dasar bagi kebijakan kesehatan masyarakat yang lebih proaktif dalam pencegahan stroke. Dengan menargetkan populasi dengan risiko tinggi, pihak berwenang dapat mengimplementasikan intervensi yang lebih efisien dan efektif.
- Peran Edukasi dan Kesadaran: Model ini dapat digunakan sebagai alat edukasi untuk meningkatkan kesadaran masyarakat tentang pentingnya deteksi dini dan pencegahan stroke. Ini dapat menciptakan budaya kesehatan yang lebih baik di masyarakat.

## Data Understanding
Dataset yang digunakan adalah dataset yang diambil dari [Kaggle](https://www.kaggle.com/fedesoriano/stroke-prediction-dataset). Dataset ini merupakan data kesehatan yang berisi informasi tentang kondisi kesehatan dan riwayat medis dari pasien yang berpotensi mengalami stroke.

Berikut informasi dari dataset :
- Dataset memiliki format CSV (*Comma-Seperated Values*).
- Dataset memiliki 5110 baris dan 12 kolom.
- Dataset memiliki 4 kolom bertipe numerik dan 8 kolom bertipe kategorikal.
- Dataset memiliki 201 baris data yang memiliki nilai null pada kolom BMI.
