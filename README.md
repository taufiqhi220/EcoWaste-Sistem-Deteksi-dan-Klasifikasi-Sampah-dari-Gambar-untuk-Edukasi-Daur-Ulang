# EcoWaste: Sistem Deteksi dan Klasifikasi Sampah dari Gambar untuk Edukasi Daur Ulang

## Ringkasan Proyek

Permasalahan sampah masih menjadi tantangan serius, terutama karena kurangnya pemahaman masyarakat tentang cara memilah dan mendaur ulang sampah dengan benar. [cite: 12] EcoWaste adalah solusi berbasis kecerdasan buatan yang bisa mengenali jenis sampah (organik, plastik, kertas) berdasarkan gambar yang diunggah pengguna. [cite: 2, 13] Proyek ini bertujuan untuk memberikan edukasi lingkungan yang simpel, cepat, dan mudah diakses, khususnya bagi generasi muda, melalui kombinasi teknologi Machine Learning (Computer Vision) dan platform digital. [cite: 14, 15] Harapannya, EcoWaste dapat membantu siapa pun belajar memilah sampah dengan mudah dan mendorong gaya hidup yang lebih peduli lingkungan. [cite: 15, 16]

## Pernyataan Masalah

Rendahnya kesadaran dan pengetahuan masyarakat tentang cara memilah sampah dengan benar (seperti organik, plastik, kertas) menyebabkan pencampuran sampah dan menyulitkan proses daur ulang. [cite: 1, 2, 3] Diperlukan solusi edukatif berbasis teknologi yang interaktif untuk membantu masyarakat mengenali dan memilah sampah secara mandiri dan praktis. [cite: 4, 5]

## Progres Saat Ini

Sejauh ini, proyek telah mencapai tahap berikut:

1.  **Pengumpulan Dataset Awal**: Dataset gambar untuk tiga kelas utama sampah (Organik, Kertas, Plastik) telah dikumpulkan. [cite: 29]
2.  **Analisis dan Pembersihan Dataset**: Dataset awal telah dianalisis untuk distribusi kelas.
3.  **Augmentasi Data**: Teknik augmentasi data telah diterapkan untuk menyeimbangkan jumlah gambar antar kelas, mengatasi ketidakseimbangan dataset awal.
4.  **Pembagian Dataset**: Dataset yang telah diaugmentasi dan diseimbangkan kemudian dibagi menjadi tiga set terpisah:
    * Set Pelatihan (Training set)
    * Set Validasi (Validation set)
    * Set Pengujian (Test set)
    Struktur folder untuk set-set ini telah dibuat (`/split_dataset/train`, `/split_dataset/validation`, `/split_dataset/test`), dengan subfolder untuk masing-masing kelas di dalamnya.

Dataset kini siap untuk digunakan dalam tahap pengembangan dan pelatihan model.

## Dataset

* **Kelas**: Organik, Plastik, Kertas [cite: 2]
* **Sumber**: Gabungan dari pengumpulan manual dan dataset publik (sesuai rencana). [cite: 49, 50]
* **Status**: Telah diaugmentasi untuk keseimbangan kelas dan dibagi menjadi set train/validation/test.

## Langkah Selanjutnya (Sesuai Rencana Proyek)

1.  **Persiapan Data untuk Model**: Memuat data dari set yang telah dibagi menggunakan `ImageDataGenerator` atau `tf.data.Dataset`.
2.  **Pembangunan Model CNN**:
    * Memilih arsitektur dasar (misalnya, VGG16, ResNet, MobileNetV2 tanpa bobot pre-trained) atau membangun CNN kustom. [cite: 31, 57]
    * Menggunakan TensorFlow dan Keras. [cite: 45, 56]
3.  **Pelatihan Model**: Melatih model menggunakan set pelatihan dan validasi. [cite: 31]
4.  **Evaluasi Model**: Mengevaluasi performa model. [cite: 31]
5.  **Pengembangan Back-End dan Front-End**: Membuat API dan antarmuka pengguna. [cite: 27, 63, 64]
6.  **Integrasi Sistem dan Pengujian**: Menggabungkan model ML dengan aplikasi web dan melakukan pengujian menyeluruh. [cite: 33, 35]

## Teknologi yang Direncanakan

* **Machine Learning**: Python, TensorFlow, Keras, OpenCV, Scikit-learn [cite: 45]
* **Back-End**: Python, Flask (atau framework lain) [cite: 45]
* **Front-End**: React.js atau HTML/CSS/JavaScript dasar [cite: 45]
* **Database**: SQLite atau PostgreSQL (sesuai kebutuhan) [cite: 45]
* **Version Control**: Git & GitHub [cite: 45]

## Cara Menjalankan (Placeholder)

Saat ini, repositori berisi skrip-skrip untuk pemrosesan data awal (augmentasi, pembagian dataset). Detail lebih lanjut mengenai cara menjalankan model dan aplikasi akan ditambahkan seiring progres proyek.

---
