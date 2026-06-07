# Komparasi Algoritma HOG-GLCM-SVM dan MobileNetV2 dalam Klasifikasi Penggunaan Helm pada Pengemudi Ojek Online Berbasis Swafoto

## Topik
Klasifikasi Citra Digital

---

## Deskripsi Proyek
Proyek ini merupakan penelitian dalam bidang computer vision yang membandingkan dua pendekatan klasifikasi citra untuk mendeteksi penggunaan helm pada pengemudi ojek online berbasis swafoto, yaitu:

- Metode tradisional: **HOG + GLCM + SVM**
- Metode deep learning: **MobileNetV2**

Tujuan utama penelitian ini adalah mengevaluasi performa kedua metode dalam mengklasifikasikan penggunaan helm, dengan fokus khusus pada aspek keselamatan kerja (*driver safety compliance*).

---

## Latar Belakang
Penerapan teknologi computer vision dalam sistem verifikasi pengemudi ojek online digunakan untuk memastikan kepatuhan terhadap standar keselamatan kerja. Salah satu komponen penting adalah deteksi penggunaan helm pada foto selfie pengemudi sebelum dapat mengaktifkan aplikasi kerja.

## Tujuan Penelitian
- Membandingkan performa HOG-GLCM-SVM dan MobileNetV2
- Menganalisis kelebihan metode tradisional vs deep learning
- Menentukan model terbaik untuk klasifikasi penggunaan helm berbasis swafoto

Namun, data swafoto memiliki beberapa tantangan, seperti:
- Variasi pencahayaan dan sudut pengambilan gambar
- Latar belakang tidak terkontrol
- Ketidakseimbangan kelas (class imbalance)
- Data duplikat yang berpotensi menyebabkan data leakage

## Metode yang Digunakan

### 1. HOG + GLCM + SVM
- **HOG (Histogram of Oriented Gradients)**: mengekstraksi fitur bentuk dan kontur
- **GLCM (Gray Level Co-occurrence Matrix)**: mengekstraksi fitur tekstur
- **SVM (Support Vector Machine)**: melakukan klasifikasi berdasarkan fitur hasil ekstraksi

### 2. MobileNetV2 
- Menggunakan arsitektur CNN ringan
- Pretrained dari ImageNet
- Dilakukan fine-tuning pada dataset helm

## Evaluasi
Evaluasi model dilakukan menggunakan metrik:
- Accuracy
- Precision
- Recall (fokus utama pada kelas *No Helmet*)
- F1-Score
