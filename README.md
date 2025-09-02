# Autoencoder-Untuk-Ekstraksi-Fitur-Data

## Konsep Singkat Autoencoder

- Apa itu Autoencoder? Ini adalah jenis neural network yang belajar "meringkas" data input menjadi representasi yang lebih ringkas (latent space), lalu rekonstruksi kembali ke bentuk asli. Bagian encoder-nya berguna untuk ekstraksi fitur (misalnya, mengurangi dimensi data dari ribuan fitur jadi puluhan).
- Kegunaan untuk Ekstraksi Fitur: Encoder bisa ambil fitur penting dari data (seperti gambar atau tabular data), berguna untuk dimensionality reduction, anomaly detection, atau preprocessing sebelum model lain.
- Dataset Contoh: Aku pakai MNIST (dataset gambar digit 0-9) karena mudah dan standar untuk demo. Kalau tugasmu pakai dataset lain, tinggal ganti aja bagian load datanya.

## Langkah-Langkah Umum

1. Load dan Preprocess Data: Ambil data, normalisasi (0-1), flatten jika perlu.
2. Bangun Model Autoencoder:
  - Encoder: Layer input → hidden layers (kurangi dimensi).
  - Decoder: Latent space → rekonstruksi ke input asli.
  - Compile dengan loss seperti MSE (Mean Squared Error) untuk rekonstruksi.
3. Train Model: Pakai data training, tanpa label (unsupervised).
4. Ekstraksi Fitur: Pakai encoder untuk ambil fitur dari data baru.
5. Evaluasi: Lihat rekonstruksi gambar atau hitung loss.

## Link Kaggle
https://www.kaggle.com/code/nailafath/ektraksi-data
