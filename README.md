# Belajar-ML-Clustering
🛍️ Customer Segmentation Analysis: Discovering Shopper Personas
🎯 Objective
Proyek ini bertujuan untuk mengelompokkan pelanggan sebuah mall ke dalam beberapa kelompok fungsional (segmen) berdasarkan profil demografis dan kebiasaan belanja mereka. Dengan memahami grup ini, bisnis dapat mempersonalisasi strategi pemasaran untuk meningkatkan retensi dan pendapatan.

📂 Dataset Overview
Data bersumber dari Mall Customer Segmentation di Kaggle. Dataset ini mencakup 200 entri pelanggan dengan fitur utama:

🆔 Customer ID: Identitas unik.

👤 Gender & Age: Profil demografis.

💰 Annual Income ($k): Pendapatan tahunan.

💳 Spending Score (1-100): Skor perilaku belanja yang ditentukan oleh pihak mal.

🛠️ Data Science Workflow
1. Exploratory Data Analysis (EDA)
Kami melakukan pembedahan data untuk melihat distribusi awal:

Zero Missing Values: Dataset sangat bersih, tidak ada nilai yang hilang.

Gender Balance: Visualisasi menggunakan Pie Chart menunjukkan distribusi antara pria dan wanita.

Statistical Summary: Rata-rata usia pelanggan adalah 38 tahun dengan skor belanja rata-rata 50.

2. Finding the "Sweet Spot" (K-Elbow)
Sebelum melakukan clustering, kami menggunakan Yellowbrick KElbowVisualizer. Alat ini membantu menentukan jumlah cluster optimal dengan mencari titik "Elbow" (siku) pada grafik inersia, memastikan model tidak overfit maupun underfit.

3. Clustering Algorithms
Kami membandingkan dan menerapkan dua pendekatan utama:

K-Means Clustering: Algoritma berbasis centroid yang efisien untuk membagi pelanggan ke dalam grup yang jelas.

DBSCAN: Algoritma berbasis kepadatan yang sangat baik dalam mendeteksi outliers atau pola yang tidak beraturan.

📊 Key Results & Evaluation
Untuk memastikan kualitas segmentasi, kami menggunakan Silhouette Score. Skor ini mengukur seberapa mirip sebuah objek dengan clusternya sendiri dibandingkan dengan cluster lainnya.

Hasil yang diharapkan biasanya mencakup:

The Big Spenders: Pendapatan tinggi & pengeluaran tinggi.

The Thrifty: Pendapatan tinggi & pengeluaran rendah.

The Average Joe: Pendapatan dan pengeluaran menengah.

⚙️ Setup & Installation
Clone the repository


git clone https://github.com/username/customer-segmentation.git

Install Dependencies


pip install pandas matplotlib seaborn scikit-learn yellowbrick


Run the Analysis Buka file sc_cluster.ipynb di Jupyter Notebook atau Google Colab dan jalankan semua sel.

💡 Tech Stack
Languages: Python

Data Manipulation: Pandas

Visualization: Matplotlib, Seaborn

ML Models: Scikit-Learn (K-Means, DBSCAN)

Diagnostics: Yellowbrick

Created with ❤️ for Data Science Enthusiasts.
