# Klasifikasi KNN pada Dataset Iris

Proyek ini mendemonstrasikan cara menggunakan algoritma **K-Nearest Neighbors (KNN)** untuk mengklasifikasikan spesies bunga dalam dataset **Iris** yang terkenal. Notebook ini mencakup implementasi dasar serta versi yang ditingkatkan dengan visualisasi yang lebih menarik.

## 📊 Dataset

**Dataset Iris** merupakan dataset yang sangat dikenal dalam pembelajaran mesin, berisi 150 sampel bunga iris dari tiga spesies yang berbeda:
- Setosa
- Versicolour
- Virginica

Setiap sampel memiliki empat fitur:
- Panjang sepal
- Lebar sepal
- Panjang petal
- Lebar petal

## 🔍 Tujuan

- Melatih model KNN untuk memprediksi spesies bunga iris.
- Mengevaluasi model menggunakan akurasi, confusion matrix, dan classification report.
- Visualisasi performa model dan hasil klasifikasi.

## ✅ Langkah-langkah

1. **Load dan Preprocessing Data**
   - Dataset diambil dari repositori UCI.
   - Fitur-fitur dinormalisasi menggunakan `StandardScaler`.

2. **Split Data Train/Test**
   - Dataset dibagi menjadi data latih (80%) dan data uji (20%).

3. **Pelatihan Model**
   - `KNeighborsClassifier` dilatih dengan `n_neighbors=5`.

4. **Evaluasi Model**
   - Prediksi dievaluasi dengan:
     - Confusion Matrix
     - Classification Report
   - Dihitung dan divisualisasikan tingkat kesalahan (error rate) untuk nilai K antara 1 sampai 39.

5. **Visualisasi yang Lebih Baik**
   - Heatmap untuk confusion matrix menggunakan Seaborn.
   - PCA digunakan untuk mengurangi dimensi dan memvisualisasikan hasil klasifikasi KNN dalam 2D.

## 📈 Hasil

- **Nilai K terbaik** ditentukan melalui grafik error rate.
- Visualisasi yang ditingkatkan membantu memahami performa klasifikasi secara lebih intuitif.

## 🛠 Dependensi

- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn

Instalasi:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn

## Referensi
UCI Machine Learning Repository – Iris Dataset
Géron, A. (2019). Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow. O'Reilly Media.
Pedregosa et al., Scikit-learn: Machine Learning in Python, JMLR 12, pp. 2825–2830, 2011.
Scikit-learn documentation – KNeighborsClassifier
Seaborn Documentation
Matplotlib Documentation
