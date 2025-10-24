# Analisis Sentimen Ulasan Aplikasi SeaBank

Proyek ini bertujuan untuk melakukan analisis sentimen terhadap ulasan pengguna dari aplikasi mobile SeaBank menggunakan algoritma machine learning dan deep learning.

## 📁 Struktur Proyek

| File | Deskripsi |
| :--- | :--- |
| `Scraping_Data (1).ipynb` | Notebook Jupyter untuk proses **pengambilan data ulasan** dari Google Play Store. |
| `ulasan_apk.csv` | Dataset **ulasan aplikasi** (mentah atau hasil *scraping*). |
| `Pelatihan_Model.ipynb` | Notebook Jupyter yang berisi langkah-langkah **preprocessing data**, **pelatihan model** analisis sentimen (kemungkinan menggunakan TensorFlow/Keras berdasarkan *snippet*), dan evaluasi model. |
| `hasil_prediksi.txt` | Contoh **hasil prediksi** sentimen dari model yang sudah dilatih. |
| `requirements.txt` | Daftar **pustaka** Python yang diperlukan untuk menjalankan proyek ini. |

***


## 🛠️ Langkah-langkah Pengerjaan

Berikut adalah alur kerja utama proyek ini:

### 1. Pengambilan Data (*Scraping*)
Data ulasan pengguna diambil dari Google Play Store menggunakan pustaka `google-play-scraper`.
* Lihat file: `Scraping_Data (1).ipynb`

### 2. Preprocessing Data dan Pelatihan Model
Data ulasan (`ulasan_apk.csv`) diproses (seperti *cleaning*, *tokenization*, *stopword removal*, *stemming* - Sastrawi digunakan berdasarkan `Pelatihan_Model.ipynb`) dan kemudian digunakan untuk melatih model klasifikasi sentimen. Model ini dilatih untuk mengklasifikasikan ulasan ke dalam kategori sentimen (misalnya, *Positive*, *Negative*, atau *Neutral*).
* Lihat file: `Pelatihan_Model.ipynb`

### 3. Prediksi dan Pengujian
Model yang sudah dilatih kemudian digunakan untuk memprediksi sentimen pada data baru atau data uji.
* Contoh hasil prediksi dapat dilihat di: `hasil_prediksi.txt`

***


