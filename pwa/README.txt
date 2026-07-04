SHIFT CALENDAR RU II DUMAI - PWA
=================================

ISI PAKET:
  index.html   - aplikasi
  manifest.json- konfigurasi PWA (nama, ikon, standalone)
  sw.js        - service worker (offline cache)
  icons/       - ikon homescreen (192, 512, maskable, apple-touch)

CARA HOSTING (sekali setup, gratis):
  1. Buat akun github.com (kalau belum)
  2. Buat repository baru, misal: shift-calendar (public)
  3. Upload SEMUA isi folder ini ke repository (drag & drop di web GitHub)
  4. Repository Settings -> Pages -> Source: "Deploy from a branch",
     branch: main, folder: / (root) -> Save
  5. Tunggu 1-2 menit. URL kamu: https://USERNAME.github.io/shift-calendar/

INSTALL DI ANDROID (Chrome):
  Buka URL -> muncul prompt "Add to Home screen" / atau menu (3 titik)
  -> "Install app". Jalan offline setelah buka pertama.

INSTALL DI IPHONE (Safari):
  Buka URL -> tombol Share -> "Add to Home Screen".
  Jalan standalone (tanpa address bar).

CATATAN:
  - Data adjustment tersimpan di perangkat (localStorage), per team,
    TIDAK sinkron antar perangkat. Pakai tombol Data -> Salin/Import
    untuk pindah perangkat.
  - Kalau update file di GitHub, app terpasang akan mengambil versi
    baru saat online (cache diperbarui otomatis oleh service worker;
    kalau bandel, tutup-buka app).
