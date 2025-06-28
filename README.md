![created](https://img.shields.io/badge/created-28/07/2024-blue)
[![Open Notebook](https://img.shields.io/badge/Open_Notebook!-blue?logo=jupyter)](https://maulanakavaldo.github.io/fruits-classification/notebook.html)
<a href="https://www.linkedin.com/in/maulana-kavaldo/" target="_blank">
  <img src="https://img.shields.io/badge/LinkedIn-blue?logo=linkedin" alt="LinkedIn">
</a>
<a href="https://www.dicoding.com/users/mkavaldo/academies" target="_blank">
  <img src="https://img.shields.io/badge/Dicoding_Profile-blue?logo=browser" alt="Dicoding Profile">
</a>

---

# Fruits Image Classification

![Fruits Image Classification](https://github.com/user-attachments/assets/f4ed00a1-d728-460c-8c34-97fbbf23e221)

## Latar Belakang:
Pengenalan gambar adalah salah satu topik penting dalam machine learning dan computer vision. Dengan kemajuan teknologi, klasifikasi gambar menjadi lebih mudah diakses dan dapat digunakan untuk berbagai aplikasi, mulai dari sistem keamanan hingga aplikasi kesehatan. Dalam proyek ini, fokus pada klasifikasi gambar buah untuk memahami bagaimana model deep learning dapat diimplementasikan untuk membedakan berbagai jenis buah.

## Permasalahan Bisnis:
Di sektor retail dan industri makanan, pengenalan buah dapat membantu dalam otomatisasi proses, seperti pengklasifikasian buah secara otomatis untuk penyimpanan, pengepakan, atau pemantauan kualitas. Dengan mengotomatisasi proses ini, bisnis dapat mengurangi kesalahan manusia, meningkatkan efisiensi operasional, dan mengurangi biaya tenaga kerja.

## Tujuan Proyek:
1. Mengembangkan model klasifikasi gambar yang mampu mengidentifikasi berbagai jenis buah dengan akurasi tinggi.
2. Menyimpan model dalam berbagai format yang kompatibel dengan berbagai platform dan perangkat.
3. Menerapkan deep learning untuk meningkatkan akurasi klasifikasi gambar.

## Cakupan Proyek
1. Mencari datatset
2. Dataset Dibagi Menjadi 80% Train Set dan 20% Test Set
3. Model Menggunakan Model Sequential, Conv2D, Pooling Layer
4. Membuat Plot Terhadap Akurasi dan Loss Model
5. Menyimpan Model ke Dalam Format SavedModel, TF-Lite dan TFJS
6. Mengimplementasikan Callback
7. Melakukan inference menggunakan salah satu model (TF-Lite, TFJS atau savedmodel dengan tf serving).

## Dataset
Dataset diperoleh dari kaggle <a href="https://www.kaggle.com/datasets/moltean/fruits" target='_blank'>Fruits Dataset</a>, yang berisi 2 folder:

1. fruits-360_dataset_100x100
2. fruits-360_dataset_original-size

Namun pada proyek ini, hanya folder **fruits-360_dataset_original-size** yang digunakan. Karena untuk mendapatkan gambar dengan resolusi yang berbeda.
Pada dataset ini terdapat 24 kelas.

## Setup environment:

1. Direkomendasikan untuk dijalankan di Google Colab

    - Upload file `notebook.ipynb` ke Google Colab 
    - Sesuaikan **BaseDir** dengan kode yang sudah ada atau sesuaikan dengan keinginanmu
    - Lakukan **run all** pada project

2. Jika dijalankan di local
    - Pastikan terhubung ke internet untuk dapat melakukan install module (library) 
    - Buka cmd atau powershell as administrator

    ```bash
    pip install -r requirements.txt
    ```
    - Buka file `notebook.ipynb` ke Google Colab 
    - Sesuaikan **BaseDir** dengan kode yang sudah ada atau sesuaikan dengan keinginanmu
    - Lakukan **run all** pada project

 ## Conclusion
 
- Berdasarkan percobaan, dihasilkan untuk:
    - Model              : Sequential
    - Akurasi            : 100 %
    - Validasi akurasi   : 100 %

    - Model              : Sequential dengan pretrained MobileNetV2
    - Akurasi            : 100 %
    - Validasi akurasi   : 100 %

   Sehingga model tersebut dapat digunakan untuk memprediksi gambar buah (_fruits_) dimasa mendatang.
- Hasil model mampu memprediksi gambar buah (fruits) yang diinputkan melalui inference.

## Saran
- Melakukan eksperimen lebih lanjut dengan menggunakan pretrained model yang tidak digunakan pada project ini. (misal VGG, ResNet dan lainnya)
- Menerapkan model ke dalam sebuah aplikasi
  
