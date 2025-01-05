# Laporan Proyek Machine Learning – Adam Gustin Wisesa
## Domain Proyek
### Latar Belakang
Kesehatan mental mahasiswa telah menjadi perhatian serius di lingkungan akademis. Tekanan akademis, sosial, dan pribadi seringkali menyebabkan stres dan gangguan kesehatan mental yang berdampak pada produktivitas dan kualitas hidup mahasiswa.

Proyek ini bertujuan untuk mengidentifikasi pola gaya hidup mahasiswa yang berkaitan dengan kesehatan mental melalui teknik clustering dalam machine learning.

### Permasalahan yang Diangkat
Bagaimana pola gaya hidup tertentu memengaruhi kesehatan mental mahasiswa, dan bagaimana mahasiswa dapat dikelompokkan berdasarkan pola tersebut untuk mendapatkan intervensi yang lebih tepat?

## Business Understanding
### Problem Statement
Pernyataan Masalah 1: Bagaimana pola tidur dan durasi istirahat memengaruhi kesehatan mental mahasiswa?<br/>
Pernyataan Masalah 2: Bagaimana kebiasaan makan dan pola aktivitas harian memengaruhi kesehatan mental?<br/>
Pernyataan Masalah 3: Bagaimana tingkat kepuasan studi berkaitan dengan kondisi mental mahasiswa?<br/>

### Goals
Jawaban Pernyataan Masalah 1: Mengidentifikasi kelompok mahasiswa dengan pola tidur yang sehat dan tidak sehat.<br/>
Jawaban Pernyataan Masalah 2: Mengelompokkan mahasiswa berdasarkan pola makan dan aktivitas fisik.<br/>
Jawaban Pernyataan Masalah 3: Menganalisis hubungan antara kepuasan studi dan kesehatan mental mahasiswa.<br/>

## Data Understanding
### Informasi Dataset
Dataset yang digunakan dalam proyek ini adalah Student Depression Dataset, yang mencakup berbagai fitur terkait pola gaya hidup dan kesehatan mental mahasiswa.<br/>
Sumber Data: https://www.kaggle.com/datasets/hopesb/student-depression-dataset<br/>
Jumlah Data: 27901 row<br/>
### Variabel Utama:
Sleep Duration: Durasi tidur harian mahasiswa.<br/>
Dietary Habits: Pola makan sehari-hari mahasiswa.<br/>
Work/Study Hours: Waktu yang dihabiskan untuk belajar atau bekerja setiap hari.<br/>
Study Satisfaction: Tingkat kepuasan mahasiswa terhadap studi mereka.<br/>

## Data Preparation
### Langkah-Langkah Data Preparation
Mengatasi missing values dengan teknik tertentu (misalnya mean imputation atau removal).<br/>
Encoding untuk fitur kategorikal seperti Dietary Habits dan Study Satisfaction.<br/>
Normalisasi fitur numerik untuk memastikan skala data seragam.<br/>
Dataset yang telah diproses siap digunakan untuk tahap modeling.<br/>

## Modeling
### Algoritma yang Digunakan:
K-Means Clustering
Menentukan jumlah cluster optimal menggunakan metode Elbow Method dan Silhouette Score.<br/>
Melakukan iterasi untuk mendapatkan hasil clustering terbaik.<br/>
Metode Inisialisasi: K-Means++

## Evaluation
### Metrik Evaluasi yang Digunakan:
Silhouette Score: Mengukur seberapa baik setiap titik data cocok dengan cluster yang ditentukan.<br/>
Inertia (Within-Cluster Sum of Squares): Menilai seberapa dekat titik data dengan pusat cluster.<br/>

### Kesimpulan Utama:
Mahasiswa dengan pola tidur buruk cenderung memiliki tingkat kepuasan studi yang rendah.<br/>
Pola makan yang tidak teratur dapat berhubungan dengan tingkat stres yang lebih tinggi.
