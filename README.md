# 📊 Sentiment Analysis of Amazon Book Reviews using PySpark

## 📌 Project Overview
Proyek ini bertujuan untuk melakukan analisis sentimen terhadap ulasan buku dari e-commerce Amazon dalam skala big data. Analisis dilakukan menggunakan PySpark, dengan preprocessing teks, ekstraksi fitur menggunakan TF-IDF, dan pemodelan menggunakan algoritma **Logistic Regression** dan **Random Forest Classifier**.

---

## 🔧 Tools and Technologies
- Apache Spark (PySpark)
- Python
- TextBlob
- TF-IDF (Term Frequency-Inverse Document Frequency)
- Logistic Regression
- Random Forest Classifier

---

## 🔍 Data Preprocessing
Langkah-langkah preprocessing data yang dilakukan:
- Menghapus data null dan duplikat
- Menghapus kolom yang tidak relevan (`asin`, `summary`, `category`)
- Text cleaning: lowercase, hapus karakter khusus
- Tokenisasi, stopwords removal, dan stemming
- Labeling sentimen menggunakan TextBlob (`Positif`, `Negatif`, `Netral`)
- Ekstraksi fitur teks menggunakan TF-IDF

---

## 📂 Dataset
Link: https://www.kaggle.com/datasets/sayedmahmoud/amazanreviewscor5?select=Books_5_part5.csv
Dataset berisi ulasan teks (`reviewText`) dari produk buku di Amazon. Setelah proses cleaning, total data yang digunakan: **5.769.068** entri.

---

## 🧠 Model
Model yang digunakan:
1. **Logistic Regression**  
   Efisien dan cocok untuk big data. Mudah diinterpretasikan dan performa sangat kompetitif setelah dikombinasikan dengan TF-IDF.
   
2. **Random Forest Classifier**  
   Model ensemble yang tangguh terhadap overfitting, mampu menangani noise dan kelas tidak seimbang, serta memberikan informasi pentingnya fitur.

---

## 📈 Evaluation Metrics
Model dievaluasi menggunakan:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**

Logistic Regression menunjukkan hasil yang lebih unggul dibandingkan Random Forest di semua metrik evaluasi.

---

## ✅ Conclusion
Logistic Regression terbukti sebagai model terbaik dalam proyek ini, dengan akurasi dan F1-score yang tinggi, serta efisiensi saat digunakan dalam kerangka kerja PySpark untuk data besar.

---

## 📚 Author
1. Bagas Eko Tjahyono Putro
2. Faiz Maula Ahmad Edwin Putra
3. Arief Muhammad Usry
