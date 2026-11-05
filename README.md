# Goldencrown Poker — Landing Page Informasional

Landing page statis HTML/CSS/JS tanpa framework. Dilengkapi 10 panduan provider pada area editorial sebelum footer, canonical, metadata Open Graph, JSON-LD WebSite, robots.txt, sitemap.xml, dan desain responsif.

## Publikasi ke GitHub Pages

1. Buat repository publik bernama `gcppoker.github.io` pada akun GitHub `gcppoker`.
2. Upload `index.html`, `robots.txt`, dan `sitemap.xml` ke root repository (jangan upload folder pembungkus saja).
3. Buka **Settings → Pages → Build and deployment**.
4. Pilih **Deploy from a branch**, branch **main**, folder **/(root)**, lalu **Save**.
5. Cek `https://gcppoker.github.io/` ketika deployment sudah berhasil.

## Penyesuaian penting

- Gunakan nama brand **Goldencrown Poker** secara konsisten.
- Jika alamat domain berubah, perbarui canonical, `og:url`, JSON-LD, sitemap.xml, dan robots.txt.
- Pastikan fakta katalog provider, promosi, dan legalitas diverifikasi sebelum menambahkan klaim baru.
- Halaman ini hanya informasional: tidak ada pembayaran, pendaftaran, atau transaksi.
- Perhatikan ketentuan GitHub Pages: tidak diperuntukkan bagi situs yang terutama memfasilitasi transaksi komersial.
- Tambahkan informasi organisasi/contact yang akurat jika tersedia, jangan membuat tautan resmi yang belum diverifikasi.

## Branding dan tombol header (revisi)

- Logo header dan footer menggunakan `https://media.spvmedapk.com/style/axhdab/desktop/img/logo-pb.png`.
- Favicon browser menggunakan `https://media.spvmedapk.com/style/axhdab/desktop/img/favicon.png`.
- Karena file gambar pada server tersebut tidak berhasil diunduh dari lingkungan pembuatan, HTML menggunakan URL eksternal langsung. Logo dan favicon akan tampil jika host tersebut dapat diakses browser pengunjung. Logo memiliki fallback teks jika gagal dimuat.
- Tombol **Daftar** dan **Login** tampil di header desktop dan mobile. URL belum diberikan, jadi tombol sengaja **belum mengarah ke website lain**.
- Untuk mengaktifkan tombol, buka `index.html`, cari `const AUTH_LINKS`, lalu isi `daftar: "https://..."` dan `login: "https://..."` dengan alamat tujuan resmi. Tombol menampilkan pemberitahuan jika URL kosong.
- Jika nanti ingin menghosting gambar secara lokal agar tidak bergantung pada server lain, unduh kedua PNG dan sesuaikan nilai `src` / `href` pada HTML.
