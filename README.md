# 🛍️ Analisis Sentimen Ulasan Aplikasi Blibli Menggunakan Support Vector Machine (SVM)

## 📖 Deskripsi Proyek

Proyek ini merupakan implementasi **Analisis Sentimen** terhadap ulasan pengguna aplikasi **Blibli** yang diperoleh melalui proses **scraping** dari **Google Play Store** menggunakan library **google-play-scraper**.

Analisis dilakukan menggunakan metode **Text Mining** dengan tahapan preprocessing, ekstraksi fitur **TF-IDF**, serta algoritma klasifikasi **Support Vector Machine (SVM)** untuk mengelompokkan ulasan ke dalam sentimen **Positif**, **Netral**, dan **Negatif**.

Proyek ini dibuat sebagai tugas **Ujian Akhir Semester (UAS)** mata kuliah **Analisis Sentimen**.

---

## 📊 Dataset

Dataset diperoleh melalui proses **scraping Google Play Store** dengan rincian sebagai berikut:

* 📱 Aplikasi : **Blibli**
* 🌐 Sumber Data : **Google Play Store**
* 📄 Jumlah Data : **1.200 ulasan**

Distribusi sentimen:

* 😊 Positif : **798**
* 😐 Netral : **35**
* 😞 Negatif : **367**

---

## ⚙️ Metodologi

Tahapan penelitian yang dilakukan:

1. 📥 Scraping Data Google Play Store
2. 🧹 Data Cleaning
3. 🔤 Case Folding
4. ✂️ Tokenizing
5. 🚫 Stopword Removal
6. 🌱 Stemming
7. 🏷️ Labeling Sentimen
8. 📑 Ekstraksi Fitur TF-IDF
9. 📊 Pembagian Data Training & Testing
10. 🤖 Training Model SVM
11. 📈 Evaluasi Model
12. 💾 Penyimpanan Model
13. 🧪 Pengujian Model

---

## 📚 Library yang Digunakan

* 🐼 Pandas
* 🔢 NumPy
* 📖 NLTK
* 🌱 Sastrawi
* 🤖 Scikit-learn
* ☁️ WordCloud
* 📊 Matplotlib
* 🎨 Seaborn
* 💾 Joblib
* 📱 Google Play Scraper

---

## 📈 Hasil Pengujian

Model **Support Vector Machine (SVM)** menghasilkan performa sebagai berikut:

### 🎯 Accuracy

**84,58%**

### 📋 Classification Report

| Sentimen | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| Negatif  | 0.79      | 0.75   | 0.77     |
| Netral   | 0.00      | 0.00   | 0.00     |
| Positif  | 0.87      | 0.93   | 0.90     |

> **Catatan:** Jumlah data sentimen netral yang sangat sedikit menyebabkan model belum mampu mengklasifikasikan kelas tersebut secara optimal.

---

## 📂 Struktur Project

```text
uas-sentiment/
Scraping_Data_Blibli.ipynb
Pemodelan_Sentimen_Blibli.ipynb
Testing_Model_Blibli.ipynb
hasil_scraping_blibli.csv
Poster_Sentimen_Ulasan_Blibli.png
svm_model.pkl
tfidf_vectorizer.pkl
README.md
```

---

## 🚀 Cara Menjalankan

### 1️⃣ Scraping Data

Jalankan notebook:

```text
1_Scraping_Data_Blibli.ipynb
```

Notebook ini akan mengambil ulasan aplikasi Blibli dari Google Play Store dan menghasilkan file:

```text
hasil_scraping_blibli.csv
```

---

### 2️⃣ Pemodelan Sentimen

Jalankan:

```text
2_Pemodelan_Sentimen_Blibli.ipynb
```

Notebook ini akan melakukan:

* Preprocessing
* Labeling
* TF-IDF
* Training SVM
* Evaluasi Model

Kemudian menghasilkan:

```text
svm_model.pkl
tfidf_vectorizer.pkl
```

---

### 3️⃣ Pengujian Model

Jalankan:

```text
3_Testing_Model_Blibli.ipynb
```

Masukkan teks ulasan, kemudian model akan memprediksi apakah ulasan termasuk:

* 😊 Positif
* 😐 Netral
* 😞 Negatif

---

## 👨‍💻 Author

**Wahyu Firman**
