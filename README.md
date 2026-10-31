# 🌸 Siklusku — Menstrual Cycle & Fertility Tracker

> Aplikasi pelacak siklus menstruasi, estimasi masa subur, dan pencatatan kesehatan reproduksi wanita yang privat, modern, dan tanpa server (*Client-Side Only*).

## 📌 Overview

**Siklusku** adalah aplikasi web interaktif yang dirancang untuk membantu pengguna memantau siklus menstruasi dan kesehatan harian secara intuitif. Aplikasi ini mengutamakan **privasi penuh**: seluruh data tersimpan secara lokal di peramban (*browser*) pengguna menggunakan `localStorage`, tanpa mengirimkan informasi sensitif ke server mana pun.

- **Live Demo / Deploy**: Integrated static deployment (GitHub Pages / Vercel)
- **Teknologi**: HTML5, Tailwind CSS (via CDN), Vanilla JavaScript (ES6+)
- **Model Data**: Offline-first via Browser `localStorage`
- **Link Akses**: https://siklusku-two.vercel.app/
---

## ✨ Fitur Utama

### 🗓️ 1. Kalkulator & Estimasi Siklus
* **Fase Menstruasi**: Menghitung proyeksi tanggal haid berikutnya dan deteksi keterlambatan.
* **Estimasi Masa Subur (Fertile Window)**: Prediksi hari ovulasi ($H - 14$ hari dari akhir siklus) serta jendela masa subur (5 hari sebelum hingga 1 hari setelah ovulasi).
* **Fase Harian**: Menampilkan informasi edukatif sesuai fase siklus yang sedang berlangsung (Folikular, Ovulasi, Luteal, Menstruasi).

### 📝 2. Jurnal & Pencatatan Harian (Daily Logging)
* **Pelacakan Suasana Hati (Mood)**: Senang, Tenang, Sensitif, Cemas, Lelah, Mudah Marah.
* **Tingkat Nyeri (Pain Scale)**: Skala intensitas nyeri dari `0` hingga `4`.
* **Intensitas Perdarahan (Flow)**: Tidak ada, Flek (*Spotting*), Ringan (*Light*), Sedang (*Medium*), Deras (*Heavy*).
* **Gejala Fisik & Catatan**: Pencatatan kustom untuk keluhan fisik harian dan catatan tambahan.

### 📊 3. Dashboard & Ringkasan Visual
* **Progress Ring Siklus**: Ringkasan visual posisi hari dalam siklus aktif.
* **Tampilan Kalender**: Riwayat dan proyeksi siklus bulanan.
* **Riwayat Log**: Panel akses cepat untuk melihat dan mengelola log kesehatan harian.

---

## 🔒 Privasi & Keamanan Data

Aplikasi ini dibangun dengan prinsip **Privacy-First**:
* **100% Client-Side**: Tidak ada autentikasi, database cloud, atau transmisi data ke server luar.
* **Penyimpanan Lokal**: Menggunakan kunci `localStorage`:
  * `siklusku_settings_v1` (konfigurasi rata-rata panjang siklus & haid)
  * `siklusku_daily_logs_v1` (riwayat log harian pengguna)
* **Ekspor & Pemulihan**: Pengguna memegang kendali penuh atas data mereka untuk mengekspor atau menghapus log kapan saja.

---

## 📁 Arsitektur Kode & Struktur File

Repositori ini memiliki arsitektur ringan tanpa *build step* yang rumit:

```
siklusku/
├── index.html        # Entry point HTML5 + UI Tailwind + Logika Vanilla JS (~100 KB)
├── metadata.json     # Manifes metadata aplikasi
└── README.md         # Dokumentasi resmi repositori
```

---

## 🚀 Cara Menjalankan Aplikasi

Aplikasi ini berbasis *Vanilla JS* tanpa memerlukan proses *compile* atau instalasi dependensi Node.js.

### Menjalankan Lokal

1. Clone repositori ini:
   ```bash
   git clone https://github.com/zakiafuadi925-ops/siklusku.git
   cd siklusku
   ```
2. Buka berkas `index.html` langsung menggunakan peramban favoritmu (Chrome, Firefox, Safari, Edge) atau gunakan ekstensi *Live Server* di VS Code.

---

## 📜 Lisensi & Hak Cipta

Dikelola dan dikembangkan oleh **[@zakiafuadi925-ops](https://github.com/zakiafuadi925-ops)**.
Bebas digunakan dan dikembangkan untuk keperluan edukasi serta referensi pribadi.
