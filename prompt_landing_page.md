# Prompt — Landing Page Aplikasi Asesmen

Paste prompt ini ke sesi baru Claude. Prompt sudah lengkap dan siap digunakan.

---

## PROMPT (salin semua teks di bawah garis ini)

---

Buatkan landing page HTML/CSS/JS lengkap dalam satu file untuk aplikasi mobile asesmen pendidikan.

## Konteks Aplikasi

Nama aplikasi: **[NAMA APLIKASI]** _(ganti dengan nama asli)_
Tagline: **Asesmen Bermakna untuk Pembelajaran yang Lebih Dalam**
Deskripsi singkat: Aplikasi asesmen interaktif untuk siswa SMP berbasis Assessment for Learning (AfL) dan Assessment as Learning (AaL) dengan pendekatan Deep Learning.

Target pengguna landing page:

- **Siswa SMP** — perlu download APK dan panduan install
- **Guru** — perlu akses ke web dashboard guru

## Struktur Halaman (urut dari atas ke bawah)

### 1. Navbar

- Logo / nama aplikasi di kiri
- Menu navigasi: Beranda · Fitur · Panduan · Tentang
- Sticky saat scroll, background blur saat di-scroll ke bawah
- Responsif: hamburger menu di mobile

### 2. Hero Section

- Headline besar: "Belajar Lebih Dalam dengan Asesmen yang Bermakna"
- Sub-headline: deskripsi singkat 1–2 kalimat
- **Dua tombol CTA utama** yang terlihat jelas dan berbeda:
  - Tombol primer: "📱 Download Aplikasi Siswa" (warna solid, menonjol)
  - Tombol sekunder: "💻 Masuk sebagai Guru" (outlined/ghost button)
- Visual dekoratif: ilustrasi atau mockup HP di sisi kanan (bisa SVG atau CSS art)

### 3. Fitur Unggulan (3 card)

- **Asesmen Interaktif** — Soal Two-Tier dengan 4 fase pengerjaan yang mendalam
- **Feedback Otomatis** — Umpan balik langsung setelah setiap jawaban
- **Portofolio Digital** — Pantau perkembangan belajar dari waktu ke waktu

### 4. Panduan Download (section penting)

Section dengan judul "Cara Download & Install Aplikasi Siswa"
Tampilkan sebagai langkah step-by-step horizontal (desktop) / vertikal (mobile):

**Step 1 — Buka Landing Page**

> Buka halaman ini di browser HP Android kamu

**Step 2 — Download APK**

> Tap tombol "Download Aplikasi Siswa" dan tunggu file terunduh

**Step 3 — Izinkan Instalasi**

> Buka Pengaturan → Keamanan → aktifkan "Instal dari sumber tidak dikenal"
> _(Langkah ini berbeda di tiap merk HP — lihat panduan lengkap di bawah)_

**Step 4 — Install & Login**

> Buka file APK yang terunduh → Install → Buka aplikasi → Login dengan akun Google

Tambahkan di bawah step:

- Tombol "📖 Lihat Panduan Lengkap" yang membuka modal/popup berisi panduan per merk HP
- Catatan kecil: "Hanya tersedia untuk Android · Ukuran ~25 MB · Gratis"

### 5. Modal Panduan Lengkap

Modal yang muncul saat tombol "Lihat Panduan Lengkap" diklik.
Berisi tab atau accordion untuk 3 merk HP paling umum:

**Samsung:**

1. Buka Pengaturan
2. Ketuk "Aplikasi" atau "Aplikasi & Notifikasi"
3. Ketuk menu ⋮ (titik tiga) → "Akses Khusus"
4. Pilih "Install aplikasi tidak dikenal"
5. Cari browser yang kamu pakai → aktifkan toggle

**Xiaomi / MIUI:**

1. Buka Pengaturan
2. Masuk ke "Privasi" → "Keamanan Khusus"
3. Ketuk "Install aplikasi tidak dikenal"
4. Aktifkan untuk browser yang kamu gunakan

**Oppo / ColorOS:**

1. Buka Pengaturan
2. Ketuk "Keamanan" → "Install aplikasi pihak ketiga"
3. Aktifkan untuk browser yang kamu gunakan

Tambahkan pesan di bawah: "Setelah install selesai, kamu bisa menonaktifkan kembali izin ini untuk keamanan."
Tombol tutup modal yang jelas.

### 6. Tentang Penelitian (section kecil)

- Judul: "Tentang Aplikasi"
- Teks singkat: aplikasi ini dikembangkan sebagai bagian dari penelitian skripsi di bidang teknologi pendidikan
- Badge/chip: "Universitas [Nama]" · "Informatika SMP" · "2025–2026"
- Nama peneliti: [NAMA PENELITI] _(ganti dengan nama asli)_

### 7. Footer

- Nama aplikasi + tagline singkat
- Link cepat: Download · Masuk Guru · Panduan
- Teks copyright: © 2026 [Nama Peneliti]. Dibuat untuk keperluan penelitian skripsi.

## Desain & Estetika

**Gaya:** Minimalis modern bertema pendidikan — bersih, terpercaya, akademis tapi tetap friendly untuk siswa SMP

**Palet warna:**

- Primary: colors: [
  Colors.deepPurple.shade900,
  Colors.deepPurple.shade600,
  Colors.deepPurple.shade400,
  ],
- Accent: kuning atau sejenisnya
- Background: Putih bersih (#FAFAFA) dengan sedikit warm tint
- Teks: Abu gelap (#1C1C1E) — bukan pure black
- Surface: Putih (#FFFFFF) dengan shadow halus

**Tipografi:**

- Heading: Font serif modern atau geometric sans yang berkarakter (bukan Inter/Roboto) — pakai Google Fonts
- Body: Font sans yang readable di semua ukuran
- Ukuran heading hero: besar dan bold, sangat menonjol

**Detail desain yang harus ada:**

- Subtle grid pattern atau dot pattern di background hero section
- Card dengan border-radius besar (16–20px) dan shadow halus
- Hover state yang smooth di semua tombol dan card
- Garis dekoratif atau shape organik sebagai aksen
- Badge/chip untuk label fitur
- Ikon SVG inline (bukan emoji) untuk fitur dan langkah panduan
- Gradient halus hanya di section tertentu — tidak berlebihan

**Animasi:**

- Fade in + slide up saat halaman pertama load (staggered per elemen)
- Smooth scroll ke section saat klik menu navbar
- Modal panduan dengan animasi masuk yang smooth
- Hover effect pada CTA tombol (subtle scale + shadow)
- Step panduan: number badge dengan animasi saat masuk viewport (Intersection Observer)

## Persyaratan Teknis

- **Satu file HTML** — CSS dan JS di dalam file yang sama menggunakan `<style>` dan `<script>`
- Tidak perlu framework — vanilla HTML/CSS/JS
- Google Fonts boleh digunakan via CDN link
- Tidak ada library JS eksternal kecuali Google Fonts
- Fully responsive: mobile (360px+), tablet (768px+), desktop (1280px+)
- Semantic HTML yang benar (main, section, nav, article, dll)
- Accessible: kontras warna WCAG AA, alt text, focus states

## Placeholder yang perlu diganti

Gunakan placeholder berikut yang mudah dicari dan diganti:

```
[NAMA APLIKASI]      → nama aplikasi yang sebenarnya
[NAMA PENELITI]      → nama peneliti/developer
[NAMA UNIVERSITAS]   → nama universitas
[URL_APK]            → URL download file APK di Firebase Storage
[URL_WEB_GURU]       → URL Flutter Web dashboard guru
[URL_BUKU_PANDUAN]   → URL PDF buku panduan (opsional, bisa # dulu)
```

## Output

Hasilkan satu file HTML lengkap yang:

1. Bisa langsung dibuka di browser dan terlihat sempurna
2. Semua fungsi berjalan (modal, smooth scroll, hamburger menu)
3. Responsif di mobile dan desktop
4. Siap di-deploy ke Vercel hanya dengan drag & drop folder
