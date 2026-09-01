# Buku Catatan Transaksi — Offline V2

Versi ini dibuat tanpa ketergantungan CDN/internet.

## Fitur offline
- Data tersimpan di localStorage perangkat.
- PWA + Service Worker.
- Bisa dibuka kembali tanpa internet setelah pertama kali dimuat melalui server lokal/HTTPS.
- Backup dan restore menggunakan JSON.
- Tidak menggunakan SheetJS/CDN.

## Cara menjalankan di HP
PWA Service Worker tidak aktif jika index.html dibuka langsung dengan `file://`.
Gunakan salah satu:
1. GitHub Pages/hosting HTTPS, buka sekali saat online, lalu aplikasi dapat dipakai offline.
2. Server lokal di HP (misalnya Termux + Python HTTP server), lalu buka alamat localhost.

## Backup
Menu Backup Data -> menghasilkan file JSON.
Untuk mengembalikan data, pilih Restore Data dan masukkan file JSON backup.

## Catatan
Data localStorage terikat pada browser/perangkat. Backup JSON secara berkala agar data aman.


V3: transaksi memiliki tanggal lengkap, status Lunas/Hutang, pelanggan transaksi, detail transaksi dan detail pelanggan yang bisa dibuka dengan mengetuk baris.
