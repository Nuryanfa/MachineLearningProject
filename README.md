# Bank Transaction Clustering and Classification

Project ini merupakan submission akhir kelas Machine Learning untuk Pemula. Dataset berisi data transaksi bank yang digunakan untuk membangun model clustering dan klasifikasi.

## Ringkasan Project

Project ini terdiri dari dua tahap utama:

1. **Clustering**
   - Melakukan exploratory data analysis.
   - Membersihkan missing value dan data duplikat.
   - Menghapus kolom ID, IP Address, dan Date.
   - Melakukan encoding fitur kategorikal.
   - Melakukan scaling fitur numerik.
   - Membangun model K-Means Clustering.
   - Menyimpan hasil clustering sebagai kolom Target.

2. **Klasifikasi**
   - Menggunakan hasil clustering sebagai target klasifikasi.
   - Melatih model Decision Tree.
   - Membandingkan dengan Random Forest.
   - Melakukan hyperparameter tuning.
   - Mengevaluasi model menggunakan accuracy, precision, recall, dan F1-score.

## Struktur File

`	ext
.
├── [Clustering]_Submission_Akhir_BMLP_NurYanfa.ipynb
├── [Klasifikasi]_Submission_Akhir_BMLP_NurYanfa.ipynb
├── bank_transactions_data_edited.csv
├── data_clustering.csv
├── data_clustering_inverse.csv
├── model_clustering.h5
├── PCA_model_clustering.h5
├── decision_tree_model.h5
├── explore_RandomForest_classification.h5
├── tuning_classification.h5
└── requirements.txt
`

## Model yang Dibangun

- K-Means Clustering
- K-Means dengan PCA
- Decision Tree Classifier
- Random Forest Classifier
- Tuned Decision Tree Classifier

## Cara Menjalankan

Install dependency:

`ash
pip install -r requirements.txt
`

Jalankan notebook secara berurutan:

1. [Clustering]_Submission_Akhir_BMLP_NurYanfa.ipynb
2. [Klasifikasi]_Submission_Akhir_BMLP_NurYanfa.ipynb

Notebook clustering menghasilkan file data_clustering.csv dan data_clustering_inverse.csv yang digunakan pada tahap klasifikasi.

## Catatan

Target klasifikasi pada project ini berasal dari hasil clustering, sehingga model klasifikasi digunakan untuk mempelajari kembali pola segmentasi yang dihasilkan oleh K-Means.
