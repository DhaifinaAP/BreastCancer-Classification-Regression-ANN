Artificial Neural Network
Repository ini dibuat guna memenuhi tugas 3 Mata Kuliah Pembelajaran Mesin

Code yang diupload melakukan proses Klasifikasi dan Regresi dataset "Breast Cancer Data Set" dengan menggunakan model ANN (Artificial Neural Network). Kemudian, dilakukan perbandingan dengan hasil klasifikasi dan regresi dengan menggunakan model SVM (Support Vector Machine).
Link Dataset : https://www.kaggle.com/datasets/erdemtaha/cancer-data

Dataset ini berisi karakteristik pasien yang terdiagnosis kanker. Dataset berisi ID unik untuk setiap pasien, jenis kanker (diagnosis), karakteristik visual kanker, dan nilai rata-rata karakteristik tersebut.

Fitur utama dari dataset adalah sebagai berikut:
1. **id**: ID unik untuk setiap pasien.
2. **Diagnosa**: Jenis kanker yang didiagnosis pada pasien (M untuk Malignant atau ganas, dan B untuk Benign atau jinak).
3. **radius_mean**: Nilai rata-rata dari radius kanker.
4. **texture_mean**: Nilai rata-rata dari tekstur kanker.
5. **perimeter_mean**: Nilai rata-rata dari perimeter kanker.
6. **area_mean**: Nilai rata-rata dari area kanker.
7. **smoothness_mean**: Nilai rata-rata dari kehalusan kanker.
8. **compactness_mean**: Nilai rata-rata dari kekompakan kanker.
9. **concavity_mean**: Nilai rata-rata dari cekungan kanker.
10. **concave points_mean**: Nilai rata-rata dari titik cekung kanker.

ada 22 fitur lain yang memiliki nilai karakteristik, jika karakteristik yang menjadi fitur utama berupa nilai rata - rata, fitur yang lain berupa nilai standard error dan worst(terburuk).

Fitur-fitur ini memberikan informasi penting tentang karakteristik visual kanker, yang sangat berguna untuk analisis dan prediksi.

## 1. Klasifikasi

Setelah dilakukan perbandingan, perbandingan akurasi model klasifikasi menggunakan SVM dan ANN adalah sebagai berikut :

akurasi model ANN = 0.9298245614035088
akurasi model SVM = 
  - kernel linear : 0.9230769230769231
  - kernel rbf    : 0.9370629370629371

## 2. Regresi

Setelah dilakukan perbandingan, perbandingan akurasi model regresi menggunakan SVM dan ANN adalah sebagai berikut :

akurasi model ANN = 
  - Root Mean Square Error (RMSE): 0.2877252969300762
  - Mean Absolute Error (MAE): 0.20938474926195647
  - R-squared (R^2): 0.9931560169398499

akurasi model SVM =
  - Root Mean Squared Error: 0.23620031140097486
  - Mean Absolute Error: 0.1523012263589766
  - R^2 Score: 0.9953839592108213

## Kesimpulan 

Berdasarkan hasil perbandingan yang telah dilakukan, dapat disimpulkan bahwa dalam kasus klasifikasi, SVM dengan kernel rbf menunjukkan performa terbaik dengan akurasi tertinggi, diikuti oleh model ANN, dan SVM dengan kernel linear memiliki akurasi yang terendah. Oleh karena itu, SVM dengan kernel rbf dapat dianggap sebagai pilihan yang optimal untuk kasus klasifikasi menggunakan dataset ini. Sementara itu, dalam konteks regresi, meskipun model ANN memiliki nilai RMSE yang lebih tinggi, model SVM menunjukkan performa yang lebih baik dengan nilai RMSE yang lebih rendah. Hal ini mengindikasikan bahwa SVM lebih unggul dalam melakukan prediksi regresi. SVM juga menampilkan nilai MAE yang lebih rendah dan R^2 yang lebih tinggi, yang menandakan bahwa secara keseluruhan, SVM memberikan hasil regresi yang lebih baik dibandingkan dengan ANN. Dengan demikian, SVM menjadi pilihan yang lebih diunggulkan dalam kasus regresi menggunakan dataset ini.

## How to run: 

### Linux :

-git clone https://github.com/DhaifinaAP/Tugas-2-Pembelajaran-Mesin-2108107010018.git

-python3 -m venv env

-source env/bin/activate

-python3 pip install -r requirements.txt

-run code Klasifikasi.ipynb dan Regresi.ipynb 

### Windows :

-git clone https://github.com/DhaifinaAP/2108107010018_Pertemuan_11_ANN.git

-python3 -m venv env

-env/Scripts/activate

pip install -r requirements.txt

-run code ANN_Classification.ipynb dan ANN_Regression.ipynb 


