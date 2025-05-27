# Prediksi Stunting Menggunakan AI Project Cycle 🤖📊

Proyek ini merupakan implementasi dari siklus proyek kecerdasan buatan (AI Project Cycle) untuk mengelompokkan dan memprediksi risiko stunting berdasarkan data kesehatan. Proyek dilakukan menggunakan **K-Means Clustering**, **SMOTE**, serta berbagai metode klasifikasi.

---

## 🚀 AI Project Cycle yang Diterapkan
1. **Problem Scoping**: Prediksi potensi stunting pada anak berdasarkan data kesehatan anak.
2. **Data Acquisition**: Menggunakan dataset stunting yang bersifat kredensial.
3. **Data Exploration**: Analisis distribusi dan korelasi pada atribut seperti tinggi badan, usia, berat badan, dll.
4. **Modelling**:
   - K-Means untuk pengelompokan awal (unsupervised) menjadi **3 cluster** berdasarkan tingkat risiko.
   - Oversampling dengan **SMOTE** untuk mengatasi imbalance.
   - Evaluasi dengan berbagai algoritma supervised.
5. **Evaluation**:
   - Model dibandingkan berdasarkan akurasi, F1-score, dan ROC-AUC.

---

## 🛠 Teknologi dan Tools
- Python (Google Colab)
- `pandas`, `scikit-learn`, `matplotlib`, `seaborn`
- KMeans, Random Forest, Logistic Regression, K-Nearest Neighbor, Gaussian Naive Bayes
- SMOTE (imbalanced-learn)

---

## 🔎 Clustering Awal dengan K-Means
- Menggunakan metode Elbow untuk menentukan jumlah cluster.
- Hasil: **3 cluster** yang mewakili risiko **Normal**, **Stunting**, dan **Overweight** stunting.
- 
---

## ⚖️ Penyeimbangan Data dengan SMOTE
- Data tidak seimbang (misal: mayoritas non-stunting)
- SMOTE digunakan sebelum proses training model klasifikasi.

---

## 🤖 Perbandingan Model Klasifikasi

| Model                 | Akurasi | F1-Score | Support |
|-----------------------|---------|----------|---------|
| Random Forest         | 98%     | 0.98     |   63    |
| SVC                   | 92%     | 0.92     |   63    |
| GaussianNB            | 87%     | 0.87     |   63    |
| LogisticRegression    | 96%     | 0.97     |   63    |
| KNeighborsClassifier  | 96%     | 0.97     |   63    |

> Random Forest menunjukkan performa terbaik secara keseluruhan.

---

## 📈 Visualisasi
- Plot cluster hasil K-Means
- Confusion Matrix tiap model
- ROC Curve
- Feature Importance (untuk Random Forest)

---

## 👤 Kontribusi
Proyek ini merupakan kolaborasi. Saya berkontribusi pada:
- Exploratory Data Analysis (EDA)
- Clustering & SMOTE
- Penerapan & evaluasi model klasifikasi
- Visualisasi & dokumentasi

---

## 📁 File yang Tersedia
- `stunting_classification.ipynb`: Training & evaluasi model
- `README.md`: Dokumentasi proyek

---

## 🌐 Sumber Data
- [SUMBER DATA BERSIFAT KREDENSIAL]

---

## 📌 Catatan
- Proyek ini bertujuan sebagai studi analisis data, bukan diagnosis medis.

