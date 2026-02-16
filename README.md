# 🕌 Islamic Wedding Invitation

Template undangan digital Islami yang cantik, interaktif, dan responsif dibangun dengan React + Framer Motion.

## ✨ Fitur Utama

### 🎨 Visual Design
- **Tema Islami Modern** - Sage green, cream, peach lembut, gold accent
- **9 Scene Lengkap** - Dari pembuka hingga penutup
- **Animasi Smooth** - Kupu-kupu terbang, parallax, scroll transition
- **Responsive Design** - Mobile first, cocok semua ukuran layar

### 🦋 Scene yang Tersedia
1. **Pembuka** - Bismillah + musik nasyid
2. **Nama Pasangan** - Ilustrasi vektor couple
3. **Detail Acara** - Tanggal, jam, lokasi dengan maps
4. **Doa Pernikahan** - Dengan ornamen kaligrafi
5. **Cerita Perjalanan** - Timeline interaktif
6. **Hadiah Digital** - QRIS + transfer bank
7. **Konfirmasi Kehadiran** - Form RSVP
8. **Ucapan Tamu** - Chat dinamis
9. **Penutup** - Quote Islami + taman

### ⚙️ Data Dinamis
Semua konten bisa diubah dari satu file JSON tanpa edit code!

## 🚀 Quick Start

### 1. Install Dependencies
```bash
npm install
```

### 2. Edit Data Undangan
Buka `src/data/invitation.json` dan ubah:
```json
{
  "namaMempelaiPria": "Nama Anda",
  "namaMempelaiWanita": "Nama Pasangan",
  "tanggal": "15 Maret 2026",
  "lokasi": "Masjid/Gedung Anda",
  ...
}
```

### 3. Jalankan Development Server
```bash
npm start
```

Aplikasi akan terbuka di `http://localhost:3000`

### 4. Build untuk Production
```bash
npm run build
```

## 📁 Struktur Project

```
islamic-wedding-invitation/
├── public/
│   └── index.html
├── src/
│   ├── components/
│   │   ├── Scene1_Opener.jsx
│   │   ├── Scene2_Names.jsx
│   │   ├── Scene3_EventDetails.jsx
│   │   ├── Scene4_Prayer.jsx
│   │   ├── Scene5_Story.jsx
│   │   ├── Scene6_Gift.jsx
│   │   ├── Scene7_RSVP.jsx
│   │   ├── Scene8_Messages.jsx
│   │   ├── Scene9_Closing.jsx
│   │   ├── Butterflies.jsx
│   │   ├── AnimatedBackground.jsx
│   │   └── ScrollTransition.jsx
│   ├── styles/
│   │   ├── global.css
│   │   └── animations.css
│   ├── data/
│   │   └── invitation.json
│   ├── App.jsx
│   └── index.js
├── package.json
└── README.md
```

## 🎨 Kustomisasi

### Mengubah Warna Tema
Di `src/data/invitation.json`:
```json
"warnaTema": {
  "primary": "#9ba88f",      // Sage green
  "secondary": "#f5e6d3",    // Cream
  "accent": "#f5a589",       // Peach
  "sky": "#b8d4e6",          // Biru langit
  "gold": "#d4af7a"          // Gold
}
```

### Menambah Vector/Ilustrasi
1. Simpan file SVG di `src/assets/vectors/`
2. Import dan gunakan di component:
```jsx
<img src="/vectors/custom.svg" alt="Description" />
```

### Menambah Audio
1. Simpan file MP3 di `src/assets/audio/`
2. Ubah path di `Scene1_Opener.jsx`:
```jsx
<audio autoPlay loop muted={!musicOn}>
  <source src="/audio/nasyid-custom.mp3" type="audio/mpeg" />
</audio>
```

## 🌐 Deploy ke Netlify

### Cara Termudah:
1. Buka [Netlify](https://netlify.com)
2. Klik **"New site from Git"**
3. Hubungkan GitHub repository ini
4. Build command: `npm run build`
5. Publish directory: `build`
6. Klik **Deploy**

### Atau gunakan Netlify CLI:
```bash
npm install -g netlify-cli
netlify deploy
```

## 📱 Browser Support
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## 🛠️ Tech Stack
- **React 18** - UI library
- **Framer Motion** - Animasi halus
- **GSAP** - Advanced animations
- **CSS3** - Styling dan responsive design

## 📝 Field Data Lengkap

```json
{
  "namaMempelaiPria": "string",
  "namaMempelaiWanita": "string",
  "tanggal": "string (format: DD Bulan YYYY)",
  "hari": "string (Senin/Selasa/etc)",
  "jam": "string (HH:MM - HH:MM WIB)",
  "lokasi": "string",
  "koordinat": "string (-6.xxxx,106.xxxx)",
  "noMasjiduul": "string",
  "jamMusholla": "string",
  "doa": "string",
  "cerita": [
    {
      "tahun": "string",
      "judul": "string",
      "deskripsi": "string"
    }
  ],
  "qris": "string",
  "noRekeningPria": "string",
  "noRekeningWanita": "string",
  "bankPria": "string",
  "bankWanita": "string",
  "namaBankPria": "string",
  "namaBankWanita": "string",
  "warnaTema": {
    "primary": "hex color",
    "secondary": "hex color",
    "accent": "hex color",
    "sky": "hex color",
    "gold": "hex color"
  }
}
```

## 🎓 Tips Penggunaan

1. **Foto Pasangan** - Ganti dengan ilustrasi vektor di `src/assets/vectors/couple.svg`
2. **Musik** - Gunakan nasyid islami yang bebas royalti
3. **Warna** - Pastikan kontras untuk aksesibilitas
4. **Mobile** - Test di berbagai ukuran layar
5. **QRIS** - Generate QRIS dari aplikasi bank Anda

## 📧 Support
Untuk pertanyaan atau issues, silakan buka GitHub issue di repository ini.

## 📄 License
MIT License - Bebas digunakan untuk keperluan pribadi maupun komersial.

---

**Dibuat dengan ❤️ untuk pasangan muslim yang bahagia**