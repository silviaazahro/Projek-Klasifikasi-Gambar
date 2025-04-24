# 🍇 Projek Machine Learning Pengembangan untuk Klasifikasi Buah Menggunakan CNN

## ⚙️ Persiapan Lingkungan

### Melalui Anaconda
```bash
conda create --name animal-classifier python=3.9
conda activate animal-classifier
pip install -r requirements.txt
```

### Melalui Terminal/Shell
```bash
pipenv install
pipenv shell
pip install -r requirements.txt
```

## 🧠 Deskripsi Proyek
Proyek ini mengembangkan model **Convolutional Neural Network (CNN)** untuk melakukan klasifikasi gambar ke dalam lima kategori buah, yaitu: **Apple, Banana, Grape, Mango, dan Strawberry**. Dataset terdiri dari **10.000 gambar** dengan resolusi yang bervariasi.

Model ini dibangun menggunakan framework TensorFlow/Keras dan hasil akhirnya dikonversi ke berbagai format seperti **SavedModel, TFLite**, dan **TensorFlow.js** agar bisa digunakan lintas platform.

## 🔧 Rangkaian Arsitektur Model

- ✅ Dibangun dengan `Sequential`, `Conv2D`, dan `MaxPooling2D`
- ✅ Memanfaatkan `EarlyStopping`, `ModelCheckpoint`, dan `ReduceLROnPlateau` untuk optimasi pelatihan
- ✅ Mencapai akurasi pelatihan dan pengujian di atas 88%
- ✅ Dataset dipecah menjadi tiga bagian: **train**, **validation**, dan **test**

## 📊 Fitur-Fitur Utama

1. **Pelatihan CNN untuk Klasifikasi 5 Jenis Buah**  
   - Melatih model agar mampu mengenali gambar apel, pisang, anggur, mangga, dan stroberi.

2. **Evaluasi Performa dan Confusion Matrix**  
   - Akurasi pada data pelatihan: 94.87%  
   - Akurasi pada data pengujian: 88.64%  
   - Confusion matrix menunjukkan performa yang konsisten di semua label.

3. **Grafik Akurasi dan Kerugian Selama Training**  
   - Visualisasi proses pelatihan untuk memantau potensi overfitting atau underfitting.

4. **Ekspor Model ke Berbagai Format**  
   - Model disimpan dalam format **SavedModel**, **TensorFlow Lite**, dan **TensorFlow.js** untuk kemudahan integrasi ke berbagai aplikasi.

5. **Prediksi Langsung dari Input Gambar**  
   - Model mampu mengidentifikasi jenis buah dari gambar yang diberikan, lengkap dengan nilai probabilitas untuk masing-masing kelas.

## 📁 Struktur Direktori

- `saved_model/` → Model dalam format TensorFlow SavedModel  
- `tflite/model.tflite` → Versi model dalam format TFLite  
- `tfjs_model/` → Versi model untuk penggunaan dengan TensorFlow.js  
- `Projek ML Pengembangan Klasifikasi.ipynb` → Notebook utama proyek  
- `requirements.txt` → Daftar dependensi Python yang dibutuhkan
