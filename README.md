# Scraping Detik.com

## Deskripsi
Repository ini berisi kode dan data hasil scraping dari portal berita Detik.com.

---

## File

### 1. scraping.ipynb
File Jupyter Notebook yang berisi
- Scraping artikel dari Detik.com.
- Preprocessing teks (lowercase, hapus tanda baca, hapus stopwords)

### 2. berita.csv
File CSV hasil scraping mentah. Berisi:
- judul, tanggal, konten, kategori

### 3. berita_final.csv
File CSV hasil preprocessing dari berita.csv. Berisi:
- judul, tanggal, konten, kategori, clean (konten yang sudah dibersihkan)

---

## Catatan
- Pastikan koneksi internet stabil selama proses scraping
- Jika terjadi error, akan melanjutkan ke artikel berikutnya
- Sesuaikan MAX_WORKERS di kode sesuai kemampuan sistem untuk meningkatkan kecepatan
