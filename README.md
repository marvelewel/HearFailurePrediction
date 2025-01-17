# ❤️ Prediksi Gagal Jantung (Heart Failure Prediction)

## 📖 Latar Belakang

Penyakit kardiovaskular merupakan penyebab utama kematian di seluruh dunia. Gagal jantung adalah kondisi serius di mana jantung tidak dapat memompa darah sebagaimana mestinya. Prediksi dini terhadap kemungkinan gagal jantung dapat membantu dalam diagnosis dan perawatan yang lebih cepat, sehingga dapat menyelamatkan nyawa.

## 🎯 Tujuan Proyek

Proyek ini bertujuan untuk membangun model prediksi gagal jantung berdasarkan dataset klinis pasien. Dengan pendekatan pembelajaran mesin, model ini dapat membantu tenaga medis dalam mengambil keputusan berdasarkan faktor-faktor kesehatan pasien.

## 📊 Dataset

Dataset yang digunakan berasal dari **Kaggle: Heart Failure Prediction Dataset**. Dataset ini berisi informasi klinis pasien yang mencakup fitur-fitur berikut:

- **Age**: Usia pasien
- **Sex**: Jenis kelamin pasien (1: Pria, 0: Wanita)
- **ChestPainType**: Jenis nyeri dada
- **RestingBP**: Tekanan darah saat istirahat (mm Hg)
- **Cholesterol**: Kadar kolesterol dalam darah (mg/dL)
- **FastingBS**: Kadar gula darah puasa (1: ≥120 mg/dL, 0: <120 mg/dL)
- **RestingECG**: Hasil elektrokardiogram saat istirahat
- **MaxHR**: Denyut jantung maksimum yang dicapai selama aktivitas fisik
- **ExerciseAngina**: Nyeri dada akibat olahraga (1: Ya, 0: Tidak)
- **Oldpeak**: Depresi ST yang diinduksi oleh olahraga relatif terhadap istirahat
- **ST\_Slope**: Kemiringan segmen ST saat latihan
- **HeartDisease**: Label target (1: Pasien menderita penyakit jantung, 0: Tidak menderita)

## 🛠️ Metode yang Digunakan

1. **Pra-pemrosesan Data**

   - Mengatasi nilai yang hilang dan data duplikat
   - Normalisasi dan encoding variabel kategorikal
   - Pemisahan data menjadi training dan testing set

2. **Model Pembelajaran Mesin**

   - **Logistic Regression**
   - **Random Forest Classifier**
   - **Support Vector Machine (SVM)**
   - **Gradient Boosting (XGBoost)**
   - **Neural Network**

3. **Evaluasi Model**

   - **Akurasi**
   - **Precision, Recall, dan F1-Score**

## 📂 Struktur Proyek

```
📁 HeartFailurePrediction
│── 📄 HeartFailurePrediction.ipynb   # Notebook utama
│── 📄 heart.csv                      # Dataset yang diambil dari kaggle
│── 📄 README.md                      # Dokumentasi proyek
```

## ⚙️ Instalasi dan Cara Menjalankan

### 1️⃣ Prasyarat

Pastikan Anda telah menginstal Python serta pustaka yang diperlukan:

```bash
pip install pandas numpy seaborn scikit-learn matplotlib xgboost
```

### 2️⃣ Jalankan Notebook

Buka Jupyter Notebook dan jalankan `HeartFailurePrediction.ipynb` untuk melihat hasil analisis secara langsung.

```bash
jupyter notebook HeartFailurePrediction.ipynb
```

## 📈 Hasil Akhir
**Evaluasi Model**:
  ```
  Model  Accuracy (5 folds)  Accuracy (10 folds)
  0  Decision Tree            0.789704             0.789736
  1            SVM            0.855099             0.851995
  ```

## 🏆 Kesimpulan

Berdasarkan hasil evaluasi model, Support Vector Machine (SVM) memiliki akurasi lebih tinggi dibandingkan Decision Tree, baik pada validasi silang 5-fold maupun 10-fold. Dengan demikian, SVM merupakan algoritma yang lebih baik dalam melakukan prediksi gagal jantung pada dataset ini.


🚀 **Terima kasih!**

