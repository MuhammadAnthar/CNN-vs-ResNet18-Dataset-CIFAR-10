# 🖼️ CIFAR-10 Image Classification: Custom CNN vs ResNet18
## 📘 Studi Kasus
Proyek ini melakukan eksperimen perbandingan antara arsitektur Custom Convolutional Neural Network (CNN) yang dimodifikasi dengan arsitektur ResNet18 (Residual Network). Fokus utama adalah mengklasifikasikan gambar kecil berwarna ($32\times32$) ke dalam 10 kategori objek yang berbeda pada dataset CIFAR-10.

## 🎯 Tujuan🛠️ Membangun model Custom CNN dengan teknik Batch Normalization dan Dropout.
- 🚀 Mengimplementasikan ResNet18 untuk melihat keunggulan Skip Connection pada jaringan dalam.
- 🧪 Melakukan Hyperparameter Tuning (Learning Rate & Batch Size) untuk mencari konfigurasi optimal.
- 📊 Menganalisis hasil melalui Confusion Matrix dan visualisasi Feature Maps (aktivitas filter pada layer).
- 
## 📊 Data
Dataset yang digunakan adalah CIFAR-10, yang terdiri dari 60.000 gambar dengan rincian:
- 10 Kelas: Airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck.
- Split Data: 45.000 (Train), 5.000 (Validation), dan 10.000 (Test).
- Preprocessing: Random Horizontal Flip, Random Crop, Normalization, dan Tensor Transformation.


## 🔄 Alur Proyek
1. 📥 Load & Preprocessing: Mengunduh dataset dan menerapkan augmentasi data.
2. 🏗️ Architecture Design: Mendefinisikan struktur Custom CNN dan modifikasi ResNet18.
3. ⚙️ Tuning: Eksperimen dengan LR (0.001 & 0.003) dan Batch Size (32 & 64).
4. 📉 Training: Proses iterasi menggunakan Cross Entropy Loss dan SGD Optimizer.
5. 📈 Evaluation: Pengujian pada data test, pembuatan grafik akurasi/loss, dan Confusion Matrix.
6. 🔍 Feature Visualization: Melihat bagaimana model "melihat" gambar melalui Feature Maps.

## 🤖 ModelingModel yang dikembangkan:
- Custom CNN: Arsitektur 3-layer konvolusi dengan peningkatan filter (64, 128, 256) + Batch Norm.
- ResNet18: Model State-of-the-Art yang diadaptasi untuk gambar ukuran $32\times32$.

## ✅ Kesimpulan 
Secara keseluruhan, ResNet18 menunjukkan performa yang lebih unggul dan stabil dengan akurasi test mencapai 82.79%. Penggunaan Skip Connections pada ResNet terbukti lebih efektif dalam menangkap fitur kompleks dibandingkan arsitektur CNN sekuensial biasa pada dataset ini.
