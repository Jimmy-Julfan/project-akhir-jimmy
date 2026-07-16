# Business Overview: JIM'S SPORT ⚡👟

**Informasi Mahasiswa**

* **Nama:** Jimmy Julfan
* **NIM:** 209250082
* **Mata Kuliah:** KAIT II
* **Dosen Pengampu:** Yoki Oktorian Sukardi S.Kom., M.A.B.

---

## 1. Nama Bisnis, Deskripsi, dan Value Proposition

**Nama Bisnis:** JIM'S SPORT — E-Commerce Sportswear Premium
**Deskripsi:** JIM'S SPORT adalah platform e-commerce berbasis *Single Page Application* (SPA) yang menyediakan koleksi pakaian dan perlengkapan olahraga premium. Platform ini dirancang untuk memberikan pengalaman berbelanja yang sangat responsif, cepat (tanpa *reload* halaman), dan memiliki antarmuka yang modern.
**Value Proposition:** - Menyediakan koleksi *sportswear* berkualitas dengan kurasi terbaik untuk pria dan wanita.

* Pengalaman berbelanja *seamless* dan interaktif dengan pembaruan keranjang belanja secara *real-time*.
* Dilengkapi sistem manajemen toko (Portal Admin) bawaan bagi pemilik bisnis untuk mengatur inventaris dan memantau stok dengan cepat.

## 2. Target Market & Segmentasi Pelanggan

* **Demografis:** Pria dan wanita (usia 18 - 35 tahun).
* **Geografis:** Masyarakat urban dan sub-urban yang memiliki akses mudah ke fasilitas olahraga atau *gym*.
* **Psikografis:** Individu dengan gaya hidup aktif, peduli pada kesehatan dan kebugaran, serta memperhatikan tren *athleisure* (pakaian olahraga untuk gaya hidup sehari-hari).
* **Segmentasi Utama:** Penggemar lari (running), praktisi yoga, member *gym*, dan masyarakat umum yang mencari kenyamanan berpakaian kasual namun tetap *sporty*.

## 3. Analisis Pasar Singkat + Kompetitor

**Analisis Pasar:** Tren *healthy lifestyle* membuat permintaan terhadap pakaian olahraga yang nyaman dan modis terus meningkat. Konsumen saat ini menginginkan proses pembelian yang tidak berbelit-belit dan visual produk yang menarik.
**Kompetitor:**

1. Toko retail olahraga fisik (Sport Station, Planet Sports) (Bisa mencoba barang langsung, namun memerlukan waktu dan usaha untuk berkunjung).
2. Official Brand Store (Nike, Adidas) (Harga sangat premium, opsi merek terbatas pada satu *brand*).
3. E-commerce general (Shopee/Tokopedia) (Pilihan sangat banyak, namun pelanggan sering kesulitan menyaring produk berkualitas tinggi di antara barang tiruan).
**Keunggulan JIM'S SPORT:** Fokus secara eksklusif pada pakaian olahraga premium dengan antarmuka web yang mulus, sistem *checkout* yang cepat, dan kurasi katalog yang tidak membingungkan pembeli.

## 4. Strategi Manajemen Produk & Katalog

* **Kategorisasi Produk:** Katalog disortir secara rapi ke dalam dua kategori utama: *Pria* dan *Wanita*. Pengguna juga dapat mengurutkan produk berdasarkan harga dan *rating*.
* **Daya Tarik Visual & UI:** Menggunakan antarmuka minimalis modern. Setiap kartu produk (*product card*) menampilkan:
* *Rating* bintang untuk membangun kepercayaan (*social proof*).
* Status ketersediaan stok yang otomatis berubah menjadi "Habis" jika stok mencapai angka 0.


* **Manajemen Inventaris (Portal Admin):** Memiliki *dashboard* admin yang diamankan dengan *login session*. Melalui panel ini, admin dapat mengubah harga, memperbarui stok, menyembunyikan produk, atau menghapus item langsung dari *browser* (berbasis *LocalStorage*).

## 5. Model Bisnis & Revenue Stream

* **Model Bisnis:** B2C (Business-to-Consumer) Retail Online.
* **Revenue Stream Utama:** Keuntungan langsung (margin) dari hasil penjualan produk *sportswear* seperti jaket lari, legging, sepatu, dan aksesoris olahraga.
* **Rencana Skalabilitas (Future):** Menambahkan sistem keanggotaan (VIP Member) untuk pelanggan setia yang memberikan akses *early bird* ke koleksi terbaru, serta ekspansi ke peralatan olahraga (dumbell, matras yoga).

## 6. Strategi Harga, Promosi, dan Diskon

* **Penetapan Harga (Pricing):** Menggunakan *Premium Pricing Strategy* yang kompetitif, merepresentasikan kualitas dan eksklusivitas produk (rentang Rp129.000 hingga Rp599.000).
* **Notifikasi Interaktif:** Menggunakan sistem *Toast Notification* saat pengguna berinteraksi dengan keranjang untuk memberikan rasa validasi instan, mendorong mereka untuk melanjutkan ke pembayaran.

## 7. Proses Checkout & Simulasi Payment Gateway

**Alur Checkout:**

1. Pelanggan memasukkan produk ke *Cart Sidebar* yang dapat diakses dari mana saja, menampilkan kalkulasi harga secara instan.
2. Saat menekan tombol "Proses Pembayaran", pelanggan diwajibkan mengisi formulir data diri lengkap (Nama, Alamat).
3. **Pilihan Metode Pembayaran:** Tersedia opsi modern seperti QRIS, Transfer Bank (BCA, Mandiri), dan E-Wallet (GoPay, DANA).
4. **Simulasi Loading:** Saat konfirmasi, muncul layar *loading overlay* "Memverifikasi Pembayaran..." selama beberapa detik.
5. **Invoice Sukses:** Stok barang otomatis terpotong di sistem, dan pelanggan menerima struk digital (Modal Berhasil) lengkap dengan ID Resi / Pesanan acak (misal: `#ORD-48291`), nama pembeli, metode, dan total bayar.

## 8. Rencana SEO, Keamanan, dan Pemeliharaan

* **SEO (Search Engine Optimization):** Menerapkan semantik tag HTML5 (`<header>`, `<section>`, `<aside>`) dan *meta viewport* yang optimal agar UI *mobile-responsive*, meningkatkan skor pencarian di Google.
* **Keamanan Front-End:** - Validasi *form* ketat (mencegah *checkout* tanpa nama, alamat, atau metode pembayaran).
* Portal Admin dilindungi dengan pengecekan `sessionStorage`, memastikan hanya pengguna dengan kredensial yang tepat (admin/admin123) yang dapat mengakses area *dashboard*.


* **Pemeliharaan Sistem:** Menggunakan arsitektur *Vanilla JavaScript* tanpa *framework* berat untuk menjaga performa muat halaman tetap cepat. Data produk saat ini menggunakan `localStorage` (`jimsport_products_v2`), dirancang agar mudah dimigrasikan ke API/Database *backend* di masa mendatang.

## 9. Rencana Penggunaan Data Analytics (Future)

* **Pelacakan Produk Populer:** Meninjau data dari *dashboard* admin (total pesanan sukses & produk terjual) untuk memahami tren gaya olahraga yang paling banyak diminati.
* **Cart Abandonment Rate:** Memantau pengguna yang memasukkan barang ke keranjang namun membatalkan proses *checkout*.
* **Tracking Pengguna Aktif:** Mengintegrasikan sistem *analytics* untuk memantau waktu kunjungan (*dwell time*) di halaman katalog untuk menilai efektivitas penataan produk.

### 📂 Struktur Folder

```text
📦 jims-sport-ecommerce
 ┣ 📂 image/          # (Aset gambar produk seperti kemeja-olahraga-pria.jpg, dll)
 ┣ 📜 index.html      # (Struktur utama halaman SPA, navigasi, dan modal)
 ┣ 📜 style.css       # (Desain UI, layout responsif, dan animasi CSS)
 ┣ 📜 script.js       # (Logika SPA, state keranjang, checkout, dan admin)
 ┗ 📜 README.md       # (Dokumentasi proyek)
