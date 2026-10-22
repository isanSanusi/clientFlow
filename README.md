# clientFlow

> Platform CRM modern untuk mengelola klien, prospek, dan alur penjualan dalam satu dasbor yang rapi dan efisien.

[React](https://img.shields.io/badge/React-19.x-61DAFB?logo=react&logoColor=black)
[Vite](https://img.shields.io/badge/Vite-6.x-646CFF?logo=vite&logoColor=white)
[Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.x-06B6D4?logo=tailwindcss&logoColor=white)
[Express.js](https://img.shields.io/badge/Express.js-5.x-000000?logo=express&logoColor=white)

## Daftar Isi

- [Gambaran Umum](#gambaran-umum)
- [Fitur Utama](#fitur-utama)
- [Teknologi](#teknologi)
- [Cara Menjalankan](#cara-menjalankan)
- [Deployment](#deployment)
- [Struktur Fitur](#struktur-fitur)
- [Rencana Pengembangan](#rencana-pengembangan)
- [Kredit](#kredit)

## Gambaran Umum

**clientFlow** adalah aplikasi Customer Relationship Management (CRM) yang dirancang untuk membantu tim penjualan dan bisnis kecil mengelola hubungan dengan klien secara lebih terstruktur.

Berbeda dengan spreadsheet yang berantakan, clientFlow menyatukan data klien, prospek (leads), kesepakatan (deals), aktivitas, dan performa penjualan dalam satu antarmuka yang bersih, cepat, dan mudah digunakan.

> **Catatan Repositori:** Repositori ini berisi artefak hasil build React untuk deployment. Aplikasi aslinya dikembangkan dengan React, Vite, Tailwind CSS, dan backend Express.js. Kode sumber lengkap dan implementasi backend mungkin berada di repositori terpisah.

## Fitur Utama

### 1. Dasbor Ringkasan
Ringkasan performa penjualan, total klien aktif, nilai pipeline, dan aktivitas terbaru dalam satu tampilan.

### 2. Manajemen Klien
- Penyimpanan data klien yang terpusat
- Riwayat interaksi dan catatan
- Status dan segmentasi klien

### 3. Manajemen Prospek & Pipeline
- Pelacakan prospek dari tahap awal hingga closing
- Visualisasi pipeline penjualan (Kanban / List)
- Indikator nilai dan probabilitas deal

### 4. Aktivitas & Tugas
- Daftar tugas, follow-up, dan pengingat
- Log aktivitas harian tim
- Status tugas: todo, in-progress, done

### 5. Antarmuka Modern
- Desain bersih dengan hierarki informasi yang jelas
- Navigasi yang cepat dan intuitif
- Responsif untuk desktop, tablet, dan ponsel

> Catatan: Fitur autentikasi, penyimpanan persisten, dan sinkronisasi real-time memerlukan backend yang aktif dan terverifikasi. Jika menggunakan data sampel, jangan diasumsikan sebagai penyimpanan permanen.

## Teknologi

### Stack Utama
- **React** - Library untuk membangun UI berbasis komponen
- **Vite** - Build tool yang cepat untuk development dan produksi
- **Tailwind CSS** - Framework CSS utility-first untuk styling yang konsisten
- **Express.js** - Backend API untuk logika bisnis dan pengelolaan data (rencana)

### Repositori Ini
Berisi hasil build produksi (HTML, CSS, JS, dan aset statis). Bukan proyek development lengkap. Konfigurasi database, environment variable, dan rute backend mungkin berada di tempat lain.

## Cara Menjalankan

### Jika hanya ada hasil build (`dist/`)

```bash
npx serve dist
```

### Jika kode sumber tersedia

```bash
# Install dependensi
npm install

# Jalankan mode development
npm run dev

# Build untuk produksi
npm run build

# Preview hasil build
npm run preview
```

## Deployment

Frontend dapat di-deploy di platform seperti **Vercel, Netlify, atau Cloudflare Pages**.

1. Atur build command: `npm run build`
2. Atur output directory: `dist`
3. Jika menggunakan client-side routing, aktifkan rewrite semua rute ke `index.html`
4. Backend Express.js harus di-deploy terpisah sebagai service atau serverless function
5. Jangan menyimpan API key atau kredensial di kode frontend. Gunakan environment variable.

## Struktur Fitur

```text
clientFlow/
├── Dashboard      # Ringkasan metrik dan aktivitas
├── Clients        # Daftar dan detail klien
├── Leads          # Manajemen prospek
├── Pipeline       # Tahapan penjualan / deals
├── Tasks          # Tugas dan follow-up
└── Settings       # Pengaturan akun dan preferensi
```

## Rencana Pengembangan

- [ ] Integrasi database persisten (PostgreSQL / MongoDB)
- [ ] Autentikasi dan otorisasi berbasis peran (Admin, Sales, Viewer)
- [ ] Fitur pencarian, filter, sorting, dan paginasi
- [ ] Ekspor data ke CSV / Excel
- [ ] Notifikasi follow-up dan pengingat otomatis
- [ ] Integrasi email dan WhatsApp untuk komunikasi klien
- [ ] Laporan penjualan dan analitik
- [ ] Mode gelap dan kustomisasi tema

## Kredit

Dibuat sebagai proyek portofolio pengembangan web yang berfokus pada alur kerja CRM, desain dasbor yang fungsional, dan pengalaman pengguna yang efisien.

Dikembangkan oleh **Ko San San**.

---
<p align="center">Dibuat untuk membuat alur kerja klien menjadi lebih mengalir — seperti namanya, clientFlow.</p>
