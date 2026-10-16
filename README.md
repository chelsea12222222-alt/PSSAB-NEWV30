# PSSAB-APP-BARU

Proyek baru aplikasi PSSAB dengan identitas Batak, warna marun-emas, logo PSSAB, dan latar Rumah Bolon.

## File utama
- `index.html`: aplikasi web dan UI.
- `config.js`: konfigurasi Supabase. Menggunakan URL dan public/publishable key yang tersedia pada proyek lama.
- `pssab-logo.png`: logo PSSAB.
- `rumah-bolon-pssab-v30.png`: gambar latar Rumah Bolon.
- `manifest.json` dan `sw.js`: dukungan PWA dasar.

## Penting sebelum dipublikasikan
1. Host seluruh isi folder ini di hosting HTTPS, misalnya GitHub Pages.
2. Uji login, pendaftaran, profil, jadwal, presensi QR, chat, dokumentasi, dan ID Card terhadap proyek Supabase yang aktif.
3. Pastikan Row Level Security (RLS) dan kebijakan izin Supabase benar untuk setiap tabel. Jangan pernah memasukkan `service_role` key ke dalam aplikasi browser.
4. Service worker hanya memberi cache aset dasar; aplikasi tetap memerlukan koneksi internet untuk Supabase.

Catatan: paket ini merupakan fondasi proyek baru yang membawa logika fitur dari file sebelumnya sebagai titik awal. Belum diklaim sebagai rilis produksi atau sudah teruji end-to-end.


## Versi 1.2 — Topbar Rumah Bolon
- Dashboard selain Beranda memakai topbar berlatar foto Rumah Bolon dengan overlay marun agar teks tetap terbaca.
- Beranda tetap menggunakan hero Rumah Bolon yang lebih besar.
- Identitas marun/emas dan motto PSSAB ditampilkan konsisten.
- Perubahan ini hanya pada lapisan tampilan; uji login dan setiap fitur setelah diterbitkan karena belum dilakukan uji end-to-end di hosting.
