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
<img width="508" alt="image" src="https://github.com/user-attachments/assets/bcbc2021-cb92-4ed6-8287-d441eca1d1b6" />



#### Learning Curve
![WhatsApp Image 2024-12-24 at 15 25 48_ab373a7d](https://github.com/user-attachments/assets/9110d657-f819-4c1b-812f-874be6d8a203)
![WhatsApp Image 2024-12-24 at 15 26 17_d11d3a8e](https://github.com/user-attachments/assets/507e8de8-4689-471e-a33d-27aef8b0e925)





#### Classification Report
![WhatsApp Image 2024-12-24 at 15 24 06_77bbabbc](https://github.com/user-attachments/assets/37fbadd4-3f8d-4ae3-938a-505fc500a01f)




#### Confusion Matrix
![image](https://github.com/user-attachments/assets/d4e34ec5-5dd7-45c5-9d10-71f72714cb9a)


Klasifikasi 0 : High Risk

Klasifikasi 1 : Low Risk

Klasifikasi 3 : Moderate Risk

### BERT
#### Preprocessing
Preprocessing data adalah langkah awal yang penting untuk menyiapkan dataset sebelum digunakan dalam model machine learning. Proses ini dimulai dengan pengecekan missing value untuk menangani data yang hilang, kemudian dilanjutkan dengan penghapusan tanda baca yang tidak relevan. Selanjutnya, case folding dilakukan untuk menyamakan seluruh teks dalam format huruf kecil agar konsisten, diikuti dengan penghapusan stopwords yang merupakan kata-kata umum yang tidak memberikan informasi signifikan. Tokenisasi kemudian digunakan untuk memecah teks menjadi unit terkecil seperti kata atau frasa. Terakhir, data dibagi menjadi dua bagian, yaitu 80% untuk pelatihan dan 20% untuk pengujian, guna memastikan model dilatih dengan baik dan diuji pada data yang belum pernah dilihat sebelumnya.


#### Classification Report
![image](https://github.com/user-attachments/assets/45a8cd30-469c-4154-855a-e12d727c8511)


#### Confusion Matrix
![image](https://github.com/user-attachments/assets/5f05723c-4884-4a86-b0b8-9e0e14f9ec09)

#### Learning Curve
![image](https://github.com/user-attachments/assets/9e5c509e-6f69-407b-9d34-f7333949d697)


Klasifikasi 0 : High Risk

Klasifikasi 1 : Low Risk

Klasifikasi 3 : Moderate Risk
