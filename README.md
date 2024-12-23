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

#### Layer yang digunakan Feedforward Neural Network
![Screenshot 2024-12-21 091611](https://github.com/user-attachments/assets/b7e07de7-0dee-43ac-97ce-d78407748903)

#### Kurva
![image](https://github.com/user-attachments/assets/4f163d14-d907-4226-8aa4-2201661ea5b5)

#### Classification Report
![Screenshot 2024-12-21 092439](https://github.com/user-attachments/assets/4c8e6e1d-725d-4379-9647-efa24e0d2385)

#### Confusion Matrix
![Screenshot 2024-12-21 092551](https://github.com/user-attachments/assets/aac290f2-a49a-477d-be4b-9b75b46f082e)
Klasifikasi 0 : Tidak

Klasifikasi 1 : Ya

### Random Forest
#### Preprocessing
Untuk Preprocessing sama seperti yang digunakan model Feedforward Neural Network. Melibatkan beberapa langkah penting untuk menyiapkan dataset agar siap digunakan dalam model machine learning. Langkah pertama adalah pengecekan missing value, yang bertujuan untuk mengidentifikasi dan menangani data yang kosong. Setelah itu, dilakukan encoding label menggunakan LabelEncoder untuk mengubah data kategori menjadi numerik, sehingga model dapat memprosesnya. Selanjutnya, normalisasi dilakukan menggunakan MinMaxScaler, yang menskalakan data numerik ke rentang [0, 1], untuk menghindari bias akibat perbedaan skala antar fitur. Terakhir, data dibagi menjadi dua bagian, yaitu 80% untuk pelatihan dan 20% untuk pengujian.

#### Classification Report
![Screenshot 2024-12-21 093341](https://github.com/user-attachments/assets/a2d020f4-cb11-4984-bbae-83d36b778539)

#### Confusion Matrix
![Screenshot 2024-12-21 093453](https://github.com/user-attachments/assets/32cf96dc-b739-48e7-aa21-095acad05449)
Klasifikasi 0 : Tidak

Klasifikasi 1 : Ya
