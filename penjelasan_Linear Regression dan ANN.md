# UTS
# Linear Regression dan ANN-Model
Penjelasan kode:
1.	Baca Dataset:

o. Dataset yang digunakan berasal dari Kaggle.

o. Data set berisikan 
"_time" = waktu pengambilan data
"temperature" = suhu yang terpantau
"Humidity" = kelembapan yang terpantau
"Heat_index" = nilai indek panas

2.	Preprocessing Data:
   
o	Kolom yang tidak relevan seperti “Unnamed : 0" dihapus.

o	Data numerik dinormalisasi menggunakan MinMaxScaler.

3.	Linear Regression:
   
o	Model regresi linear (LinearRegression) diuji dengan membagi data menjadi train dan test set.

o	Skor akurasi pada data train dan test ditampilkan.

4.	Artificial Neural Network (ANN):
   
o	Model jaringan saraf tiruan (ANN) dengan dua lapisan (32 neuron pada lapisan pertama dan 1 neuron pada lapisan kedua) dibuat.

o	Fungsi aktivasi yang digunakan adalah ReLU pada lapisan pertama dan linear pada lapisan kedua.

o	Model di-compile dengan optimizer Adam dan loss function mean squared error.

Hasil Linear Regression:

•	Train score 0.997827613764311

•	Test score 0.9977907105621123

Hasil ANN:

•	Model ANN telah dievaluasi pada data test.

•	nilai evaluasi dari X_test, y_test adalah 1.8355189013163908e-06, 0.0010202040430158377.

5.	Perbandingan Prediksi Linear Regression dan ANN:
   
o	Scatter plot menunjukkan perbandingan antara nilai aktual dan nilai prediksi menggunakan regresi linear dan ANN.

o	Garis putus-putus abu-abu menunjukkan nilai aktual dan prediksi yang sama.

Hasil dari kode menunjukkan beberapa hal:

1.	Grafik Training dan Validasi Loss:
   
o	Grafik ini menggambarkan training loss (garis merah) dan validation loss (garis hijau) selama proses pelatihan model.

o	Titik biru menunjukkan epoch terbaik dengan validation loss terendah.
(Semakin rendah validation loss, semakin baik performa model. Pada titik biru, model memiliki performa optimal)

2.	Grafik Training dan Validasi Akurasi:
   
o	Grafik ini membandingkan training accuracy (garis merah) dengan validation accuracy (garis hijau) selama proses pelatihan model.

o	Titik biru menunjukkan epoch terbaik dengan validation accuracy tertinggi.
(Semakin tinggi validation accuracy, semakin baik performa model. Pada titik biru, model memiliki akurasi optimal)

3.	Hasil Regresi Linear:
   
o	Skor R2 pada data test: 0.9978 .
(Model regresi linear sangat baik dalam memprediksi )

4.	Hasil Artificial Neural Network (ANN):
   
o	Model ANN telah dievaluasi pada data test.

o   Skor R2 pada data test: 0.9999
(Model ANN memiliki performa yang baik)

5.	Perbandingan Prediksi Linear Regression dan ANN:
   
o.  Presentase akurasi yang paling besar adalah model ANN

o.  99.99% > 99.78%

O.  Metode ANN dapat melakukan tugasnya dengan baik, maka disarankan untuk menggunakan metode ini daripada linear regression


