# Web Scraper untuk Berita Detik.com

Proyek ini berisi sebuah skrip Python yang dirancang untuk melakukan *web scraping* pada situs berita populer Indonesia, **Detik.com**. Skrip ini secara otomatis mengumpulkan judul berita, kategori, dan waktu publikasi, lalu menyimpannya ke dalam format file CSV.

---

## Daftar Isi

1.  [Latar Belakang](#latar-belakang)
2.  [Fitur Utama](#fitur-utama)
3.  [Tech Stack](#tech-stack)
4.  [Cara Penggunaan](#cara-penggunaan)
5.  [Format Output](#format-output)

---

## Latar Belakang

Mengumpulkan data dari situs berita adalah langkah fundamental dalam banyak proyek analisis data, seperti analisis sentimen, pemodelan topik, atau pemantauan tren. Proyek ini dibuat untuk menyediakan alat yang sederhana namun efektif untuk mengotomatisasi proses pengumpulan data berita dari salah satu sumber berita digital terbesar di Indonesia.

## Fitur Utama

-   **Scraping Dinamis**: Mengambil data dari halaman utama Detik.com.
-   **Ekstraksi Data Spesifik**: Mengumpulkan informasi penting seperti **judul berita**, **kategori** (misalnya, 'Finance', 'Sport'), dan **waktu publikasi**.
-   **Penyimpanan Otomatis**: Hasil scraping secara otomatis disimpan ke dalam file `detik_populer.csv` untuk analisis lebih lanjut.
-   **Kode yang Mudah Dimengerti**: Skrip ditulis dengan cara yang sederhana dan diberi komentar agar mudah dipahami dan dimodifikasi.

---

## Tech Stack

-   **Bahasa Pemrograman**: Python
-   **Library Utama**:
    -   `requests`: Untuk mengirim permintaan HTTP ke server Detik.com.
    -   `BeautifulSoup4`: Untuk mem-parsing konten HTML dan mengekstrak data.
    -   `pandas`: Untuk mengelola data yang telah di-scrape dan menyimpannya ke file CSV.

---

## Cara Penggunaan

Untuk menjalankan skrip ini di lingkungan lokal Anda, ikuti langkah-langkah berikut:

1.  **Clone Repositori Ini**
    ```bash
    git clone https://github.com/haaahabib/scraping-detik.com.git
    ```

2.  **Masuk ke Direktori Proyek**
    ```bash
    cd scraping-detik.com
    ```

3.  **Install Library yang Dibutuhkan**
    ```bash
    pip install requests beautifulsoup4 pandas
    ```

4.  **Jalankan Skrip Scraper**
    ```bash
    python detik.py
    ```

Setelah skrip selesai dijalankan, sebuah file bernama `detik_populer.csv` akan dibuat di dalam direktori yang sama.

---

## Format Output

Data yang berhasil di-scrape akan disimpan dalam file `detik_populer.csv` dengan kolom-kolom sebagai berikut:

| Nama Kolom | Deskripsi |
| :--- | :--- |
| **judul** | Judul lengkap dari artikel berita. |
| **kategori** | Kategori berita (contoh: 'detikNews', 'detikFinance'). |
| **waktu** | Waktu kapan berita tersebut dipublikasikan. |
