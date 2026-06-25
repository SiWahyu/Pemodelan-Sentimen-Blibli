# Analisis Sentimen Review Aplikasi Blibli Menggunakan Support Vector Machine (SVM)

## Deskripsi Proyek

Proyek ini merupakan implementasi Analisis Sentimen terhadap ulasan pengguna aplikasi Blibli yang diperoleh dari Google Play Store. Analisis dilakukan menggunakan metode Text Mining dengan ekstraksi fitur TF-IDF dan algoritma klasifikasi Support Vector Machine (SVM).

Proyek ini dibuat untuk memenuhi tugas Ujian Akhir Semester (UAS) Analisis Sentimen.

## Dataset

Dataset yang digunakan berupa ulasan pengguna aplikasi Blibli yang telah diberi label sentimen:

- Positif : 400 data
- Netral : 400 data
- Negatif : 400 data

Total dataset: 1200 ulasan.

## Metodologi

Tahapan yang dilakukan pada penelitian ini:

1. Pengumpulan Dataset
2. Data Cleaning
3. Text Preprocessing
4. Stopword Removal
5. Ekstraksi Fitur TF-IDF
6. Pembagian Data Training dan Testing
7. Training Model SVM
8. Evaluasi Model
9. Penyimpanan Model
10. Pengujian Model

## Library yang Digunakan

- Pandas
- NumPy
- NLTK
- Scikit-learn
- WordCloud
- Matplotlib
- Seaborn
- Joblib

## Hasil Pengujian

Model Support Vector Machine (SVM) menghasilkan:

- Accuracy : 65.83%

Classification Report:

| Sentimen | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| Negatif  | 0.68      | 0.64   | 0.66     |
| Netral   | 0.56      | 0.46   | 0.51     |
| Positif  | 0.71      | 0.88   | 0.78     |

## Struktur File

```text
Pemodelan_Sentimen_Blibli.ipynb
blibli_reviews_balanced_1200.csv
svm_model.pkl
tfidf_vectorizer.pkl
README.md
```

## Cara Menjalankan

1. Buka file `Pemodelan_Sentimen_Blibli.ipynb`
2. Jalankan seluruh cell secara berurutan
3. Model akan menghasilkan file:
   - `svm_model.pkl`
   - `tfidf_vectorizer.pkl`

4. Model akan menjalankan kode Pengujian Model Review Positif dan Negatif

## Author

Wahyu Firman
