# Klasifikasi Gambar Kucing dan Anjing

## Deskripsi Proyek
Proyek ini bertujuan untuk membangun model klasifikasi gambar untuk membedakan antara gambar **Kucing** dan **Anjing** menggunakan Convolutional Neural Network (CNN) yang dibuat dengan TensorFlow dan Keras.

Model dilatih pada dataset yang berisi 25000 gambar (12500 Anjing dan 12500 Kucing) dengan augmentasi data dan menggunakan callback `EarlyStopping` serta penyesuaian `class_weight` untuk mengatasi ketidakseimbangan data. Model kemudian dikonversi ke dalam tiga format:
- SavedModel (untuk TensorFlow Serving)
- TFLite (untuk aplikasi mobile atau embedded)
- TensorFlow.js (untuk aplikasi berbasis web)

## Cara Menjalankan
1. **Notebook** (`notebook.ipynb`) digunakan untuk training dan konversi model.
2. **Model SavedModel** bisa digunakan untuk inference menggunakan `keras.layers.TFSMLayer`.
3. **Model TFLite** dapat digunakan dalam aplikasi Android atau embedded system.
4. **Model TensorFlow.js** dapat digunakan pada aplikasi web.

### Contoh Inference di Notebook dapat dilihat pada file "Dogs VS Cats Inference.ipynb".

