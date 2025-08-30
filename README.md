# Aplikasi Absensi Harian Pegawai
Aplikasi absensi sederhana berbasis HTML/CSS/JavaScript untuk **SMK Negeri 10 Jeneponto**.

## Fitur
- Input nama, status kehadiran, jam datang, dan jam pulang
- Tabel rekap otomatis
- **Export ke CSV**
- **Print langsung dari browser**
- Desain responsif dengan stylesheet cetak (print)

## Struktur Folder
```
smkn10-absensi/
├─ index.html
├─ css/
│  └─ styles.css
├─ js/
│  └─ app.js
├─ assets/
│  └─ logo.png     ← (opsional) letakkan logo sekolah di sini
├─ .github/
│  └─ workflows/
│     └─ deploy.yml   ← workflow GitHub Pages (lihat di bawah)
├─ LICENSE
├─ README.md
└─ .gitignore
```

## Cara Pakai (Lokal)
1. Buka **index.html** di browser.
2. Isi form, klik **Simpan Absensi**, data akan tampil di tabel.
3. Klik **Export ke CSV** untuk mengunduh rekap, atau **Print** untuk cetak.

## Deploy ke GitHub Pages
1. Buat repository baru di GitHub, misalnya `smkn10-absensi`.
2. Upload seluruh isi folder ini ke repository.
3. Aktifkan GitHub Pages lewat **Settings → Pages → Build and deployment → GitHub Actions**.
4. Commit dan push, tunggu workflow selesai. Aplikasi akan tampil di URL GitHub Pages repo Anda.

## Ganti Logo
- Secara default index.html memakai URL logo online.
- Jika ingin memakai file lokal, simpan gambar sebagai `assets/logo.png` lalu ubah tag img di `index.html` menjadi:
  ```html
  <img src="assets/logo.png" alt="Logo Sekolah" class="logo" />
  ```

## Lisensi
MIT © 2025 SMK Negeri 10 Jeneponto
