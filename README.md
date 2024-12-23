Nama : Zahra Sabilla Usman

NIM : 202110370311337

Machine Learning A

![IMG_20240210_102118](https://github.com/user-attachments/assets/c28fb384-8803-44f6-bc63-b9daf1df6290)



# Efektivitas Obat-obatan 
  Alat atau bahan yang digunakan untuk mendiagnosis, mencegah, mengobati, atau meredakan gejala penyakit disebut obat. Obat adalah salah satu cara utama untuk mempertahankan dan memulihkan kesehatan dalam dunia medis. Jenis obat sangat beragam, mulai dari antibiotik untuk memerangi infeksi bakteri, analgesik untuk meredakan nyeri, hingga obat khusus seperti antidepresan untuk gangguan mental atau insulin untuk diabetes. Obat-obatan semuanya dibuat dengan cara farmakologis tertentu untuk membantu tubuh melawan penyakit atau memperbaiki fungsi fisiologis yang terganggu. Namun, sejumlah variabel, termasuk kondisi pasien, dosis yang diberikan, dan kepatuhan pasien terhadap anjuran penggunaan, sering kali memengaruhi kinerja obat. Oleh karena itu, untuk memastikan manfaat obat-obatan secara keseluruhan, evaluasi efektivitasnya melalui analisis pengalaman atau ulasan pasien sangat penting.
  
## Dataset
  Proyek ini menggunakan dataset dari Kaggle (https://www.kaggle.com/code/harshjain123/drugs-review-sentiment/input) yang terdiri dari 53.765 data. Dengan memanfaatkan model prediksi seperti Long Short Term Memory (LSTM) dan BERT, analisis data dapat dilakukan dengan lebih cepat dan akurat. Proyek ini bertujuan untuk melihat efektivitas obat, dilihat dari review dan rating pengguna.
  
## Long-short Term Memory architecture
![1_oJcSMhQZA3vr0P-kXz0SYA](https://github.com/user-attachments/assets/3b78218b-292a-4c5e-a7bd-0b205644e0e7)

## BERT architecture
![Overview-of-the-proposed-BERT-LSTM-model-Pooling-Module-is-responsible-for-connecting](https://github.com/user-attachments/assets/6162c18d-98c4-4fd7-89cc-e14f635a65f0)

## Modelling
### Long-Short Term Memory
#### Preprocessing
Preprocessing data adalah langkah awal yang penting untuk menyiapkan dataset sebelum digunakan dalam model machine learning. Proses ini dimulai dengan pengecekan missing value untuk menangani data yang hilang, kemudian dilanjutkan dengan penghapusan tanda baca yang tidak relevan. Selanjutnya, case folding dilakukan untuk menyamakan seluruh teks dalam format huruf kecil agar konsisten, diikuti dengan penghapusan stopwords yang merupakan kata-kata umum yang tidak memberikan informasi signifikan. Tokenisasi kemudian digunakan untuk memecah teks menjadi unit terkecil seperti kata atau frasa. Terakhir, data dibagi menjadi dua bagian, yaitu 80% untuk pelatihan dan 20% untuk pengujian, guna memastikan model dilatih dengan baik dan diuji pada data yang belum pernah dilihat sebelumnya.

#### Layer yang digunakan Long-Short Term Memory
![image](https://github.com/user-attachments/assets/952f70b4-10d1-4709-9c61-c13cccc1f87d)


#### Distribusi pelabelan
![image](https://github.com/user-attachments/assets/8dfd9c6f-1a66-425c-8d32-c2e9009411f4)


#### Classification Report
![image](https://github.com/user-attachments/assets/821d693d-5e15-4cbe-8660-2e9a0443f23b)

#### Confusion Matrix
![image](https://github.com/user-attachments/assets/3d98fd93-c199-4574-b5d2-7e3b2d639225)

Klasifikasi 0 : High Risk

Klasifikasi 1 : Low Risk

Klasifikasi 3 : Moderate Risk

### BERT
#### Preprocessing
Preprocessing data adalah langkah awal yang penting untuk menyiapkan dataset sebelum digunakan dalam model machine learning. Proses ini dimulai dengan pengecekan missing value untuk menangani data yang hilang, kemudian dilanjutkan dengan penghapusan tanda baca yang tidak relevan. Selanjutnya, case folding dilakukan untuk menyamakan seluruh teks dalam format huruf kecil agar konsisten, diikuti dengan penghapusan stopwords yang merupakan kata-kata umum yang tidak memberikan informasi signifikan. Tokenisasi kemudian digunakan untuk memecah teks menjadi unit terkecil seperti kata atau frasa. Terakhir, data dibagi menjadi dua bagian, yaitu 80% untuk pelatihan dan 20% untuk pengujian, guna memastikan model dilatih dengan baik dan diuji pada data yang belum pernah dilihat sebelumnya.

#### Classification Report
![image](https://github.com/user-attachments/assets/ee7af99c-76c7-4bd5-b08d-6e1d1e184ea6)


#### Confusion Matrix
![image](https://github.com/user-attachments/assets/5f05723c-4884-4a86-b0b8-9e0e14f9ec09)

Klasifikasi 0 : High Risk

Klasifikasi 1 : Low Risk

Klasifikasi 3 : Moderate Risk
