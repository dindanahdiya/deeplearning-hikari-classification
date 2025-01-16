# **Deep Learning Hikari Classification** 
## **Deskripsi Proyek**
Proyek ini bertujuan untuk klasifikasi multi-kelas traffic category jaringan menggunakan HIKARI 2021 All Flow Meter Dataset. Model yang digunakan adalah **Multi-Layer Perceptron** dengan arsitektur yang mencakup dropout layers, batch normalization, dan softmax activation function.

Otomatisasi pengambilan dataset dan preprocessing dilakukan menggunakan KaggleHub, yang meningkatkan efisiensi dan reproduktibilitas model. Teknik **Random Over Sampling** diterapkan untuk mengatasi ketidakseimbangan kelas dalam dataset.

## **Fitur Utama**
-  Dataset: HIKARI 2021 All Flow Meter Dataset
-  Model: Deep Learning dengan Multi-Layer Perceptron (MLP)
-  Teknik Balancing Data: Random Over Sampling
-  Famework: TensorFlow / PyTorch
-  Otomatisasi: KaggleHub untuk otomatisasi dataset retrieval dan preprocessing
-  Evaluasi: Akurasi model mencapai 90%, dengan beberapa kelas mencapai F1-score 99%

## **Hasil dan Evaluasi**
Model diuji menggunakan akurasi, precision, recall dan F1-score. Hasil evaluasi menunjukkan sebagai berikut:
| **Class**                  | **Precision** | **Recall** | **F1-Score** |  
|----------------------------|--------------|------------|-------------|  
| **Benign (0)**             | 0.79         | 0.86       | 0.82        |  
| **Background (1)**         | 0.82         | 0.56       | 0.66        |  
| **Probing (2)**            | 0.98         | 1.00       | 0.99        |  
| **Bruteforce (3)**         | 0.99         | 1.00       | 0.99        |  
| **Bruteforce-XML (4)**     | 0.85         | 1.00       | 0.92        |  
| **XMRIGCC CryptoMiner (5)**| 0.98         | 1.00       | 0.99        |  
| **Overall Accuracy**       | -            | -          | **0.90**    |  

* Catatan: Model memiliki kesulitan dalam mengklasifikasikan kategori Background, menunjukkan perlunya penyempurnaan lebih lanjut dalam pemilihan fitur atau balancing data.

## **Hasil dan Evaluasi**
Untuk meningkatkan model ini, beberapa langkah pengembangan yang dapat dilakukan:
1. Feature Engineering, menggunakan PCA atau t-SNE untuk meningkatkan pemisahan kelas.
2. Ensemble Learning, menerapkan metode seperti Gradient Boosting atau Stacking untuk meningkatkan akurasi.
3. Teknik Balancing Lanjutan, menggunakan SMOTE atau Cost-Sensitive Learning sebagai alternatif Random Over Sampling.
4. Optimasi Hyperparameter, menerapkan Bayesian Optimization atau Evolutionary Algorithms untuk pencarian hyperparameter yang lebih efisien.
5. Analisis Error Lebih Lanjut, memeriksa confusion matrix untuk mengidentifikasi pola kesalahan dan memperbaikinya.
