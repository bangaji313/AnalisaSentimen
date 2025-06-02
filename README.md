# AnalisaSentimen
Proyek ini bertujuan untuk membangun model analisis sentimen terhadap ulasan aplikasi **Wondr by BNI** yang diambil dari Google Play Store. Dataset yang digunakan terdiri dari **10.000 sampel acak** dari total lebih dari 39.000 review yang berhasil dikumpulkan melalui proses scraping.

Beberapa tahapan penting yang telah dilakukan:

- **Preprocessing**: Normalisasi, tokenisasi, stopword removal, stemming, dan pelabelan sentimen.
- **Ekstraksi fitur** menggunakan dua pendekatan:
  - TF-IDF (Term Frequency - Inverse Document Frequency)
  - Word2Vec (Word Embedding)
- **Pelatihan model** dilakukan menggunakan empat skema kombinasi:
  1. Logistic Regression + TF-IDF (80/20)
  2. Random Forest + Word2Vec (80/20)
  3. SVM + TF-IDF (70/30)
  4. Deep Learning (Sequential Model) + TF-IDF (80/20)
- **Evaluasi model** berdasarkan metrik:
  - Akurasi
  - Presisi
  - Recall
  - F1-Score
- **Inference**: Model digunakan untuk mengklasifikasikan 10 kalimat ulasan baru secara otomatis.

### Hasil Akhir
- Model terbaik secara umum adalah **Logistic Regression dengan TF-IDF (80/20)** karena memiliki akurasi tinggi dan presisi terbaik di antara semua model.
- Model Deep Learning menunjukkan performa kuat, namun memerlukan lebih banyak sumber daya dan waktu pelatihan.

---

Proyek ini merupakan bagian dari **Submission 1 - Belajar Fundamental Deep Learning** pada platform **Dicoding Indonesia** dalam rangka program **Coding Camp 2025 by DBS Foundation**
