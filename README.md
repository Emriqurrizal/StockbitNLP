# StockbitNLP (Google Colab Notebooks)

Repo ini berisi notebook NLP yang **dirancang untuk dijalankan di Google Colab**.

## Kenapa ditargetkan untuk Google Colab?
Notebook di folder `Notebooks/` mengikuti pola eksekusi Colab, misalnya:
- Menggunakan path seperti **`/content/...`** (default working directory di Colab).
- Melakukan instalasi dependency langsung di notebook memakai `!pip install ...`.
- Memanfaatkan **GPU** yang tersedia di Colab untuk proses yang lebih berat (contoh: embedding menggunakan TensorFlow Hub).

## Cara menjalankan di Google Colab
1. Buka Google Colab: https://colab.research.google.com/
2. Upload notebook dari folder `Notebooks/` (menu **File → Upload notebook**), atau buka via GitHub.
3. Pastikan dataset CSV tersedia di environment Colab:
   - Cara cepat: upload file CSV ke sesi Colab (panel kiri → **Files** → **Upload**), sehingga file berada di `/content/`.
   - Alternatif: mount Google Drive jika file besar / ingin persist.

### Contoh penempatan dataset
Beberapa notebook membaca dataset dengan pola seperti:
- `/content/stockbit_reviews_sentiment.csv`

## Struktur folder
- `Notebooks/` — kumpulan notebook utama
- `csv/` — dataset hasil scraping/cleaning (untuk penggunaan lokal atau saat ingin upload ke Colab)

## Daftar notebook
- `Notebooks/stockbit_scraping.ipynb`
- `Notebooks/stockbit_preprocessing.ipynb`
- `Notebooks/stockbit_EDA.ipynb`
- `Notebooks/stockbit_TFIDF.ipynb`
- `Notebooks/stockbit_sentiment_analysis.ipynb`

