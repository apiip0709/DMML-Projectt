# Laporan Proyek DMML / Stroke Risk Prediction

## Kelompok 10
- A. Afif Alhaq - H071221064
- Adrian Hidayat - H071221091
- Evan Pandu - H071221057
- Muhammad Rifky Aqid - H071211077

## Structure
📦DMML-Projectt
 - ┣ 📂assets
 -   ┗ 📜!Screenshot 2024-06-28 101134.png
 -   ┗ 📜!Screenshot 2024-06-28 101225.png
 -   ┗ 📜!Screenshot 2024-06-28 101741.png
 - ┣ 📂dataset
 - ┃ ┗ 📜stroke-data.csv
 - ┣ 📂models
 - ┣ ┣ 📜dt.sav
 - ┣ ┗ 📜scaler.pkl
 - ┣ 📂report
 - ┃ ┗ 📜DMML-Kelompok 10 Report (PPT).pdf
 - ┃ ┗ 📜Paper Kelompok 10 - DMML.pdf
 - ┣ 📂templates
 - ┃ ┗ 📜home.html
 - ┃ ┗ 📜nostroke.html
 - ┃ ┗ 📜stroke.html
 - ┣ 📜app.py
 - ┗ 📜data stroke prediction.ipynb
 - ┗ 📜README.md

## Dataset
Dataset yang digunakan adalah dataset yang diambil dari [Kaggle](https://www.kaggle.com/fedesoriano/stroke-prediction-dataset). Dataset ini merupakan data kesehatan yang berisi informasi tentang kondisi kesehatan dan riwayat medis dari pasien yang berpotensi mengalami stroke.

Berikut informasi dari dataset :
- Dataset memiliki format CSV (*Comma-Seperated Values*).
- Dataset memiliki 5110 baris dan 12 kolom.
- Dataset memiliki 4 kolom bertipe numerik dan 8 kolom bertipe kategorikal.
- Dataset memiliki 201 baris data yang memiliki nilai null pada kolom BMI.

## Reporting PPT dan Laporan
- [Link Report PPT](https://drive.google.com/file/d/1SmzOWOYucUSXcQq5QqlDaYaZ07tnggZx/view?usp=sharing)

- [Link Paper Final Report](https://drive.google.com/file/d/1xJ-S4PByIfKby8n6pY2_hO8ZKrma3mgH/view?usp=sharing)

## Menjalankan Aplikasi
- Lakukan clone terhadap hasil fork repository ini ke komputer kalian
  ```
  git clone https://github.com/apiip0709/DMML-Projectt.git
  ```
- Buka Terminal Pada File yang sudah di clone, lalu jalankan perintah berikut:
  ```
  python app.py
  ```

## Tampilan Aplikasi
- Tampilan Awal berisi variable yang memengaruhi Penyakit Stroke
![alt text](<assets/Screenshot 2024-06-28 101134.png>)

- Tampilan jika diagnosa stroke ada
![alt text](<assets/Screenshot 2024-06-28 101741.png>)

- Tampilan jika diagnosa stroke tidak ada
![alt text](<assets/Screenshot 2024-06-28 101225.png>)

