# Aplikasi Administrasi Guru AI (EdAdmin Pro)

Sistem Administrasi Guru Digital terintegrasi Asisten AI, Perangkat Ajar Kurikulum Merdeka & KBC, Presensi QR Code, serta Database Cloud Firebase.

## Cara Menjalankan di Lokal (Komputer)

1. Install dependencies:
   ```bash
   npm install
   ```
2. Buat file `.env` (salin dari `.env.example`) dan isi `GEMINI_API_KEY`:
   ```env
   GEMINI_API_KEY="AIzaSy..."
   ```
3. Jalankan server development:
   ```bash
   npm run dev
   ```

## Cara Deploy ke GitHub & Vercel

1. Unggah seluruh isi folder ini ke repository **GitHub** Anda.
2. Buka [Vercel](https://vercel.com/) -> **Add New Project** -> Import repository GitHub tersebut.
3. Di bagian **Environment Variables** pada Vercel, tambahkan:
   - `GEMINI_API_KEY` = *(API Key Google Gemini Anda)*
4. Klik **Deploy**.
5. Setelah mendapatkan URL Vercel (misal `nama-aplikasi.vercel.app`), buka **Firebase Console** -> **Authentication** -> **Settings** -> **Authorized domains** -> Tambahkan domain Vercel Anda agar fitur Login Google berjalan lancar.
