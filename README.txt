# Aplikasi Jadual Guru — prototaip

## Fail
- `index.html`: aplikasi web (HTML, CSS, JavaScript).
- `manifest.webmanifest`: metadata pemasangan PWA.
- `sw.js`: cache asas untuk penggunaan luar talian selepas fail dimuat turun.
- `contoh-jadual.json`: data contoh yang boleh diimport.

## Cara menjalankan dengan paling mudah
1. Nyahzip folder ini.
2. Buka `index.html` dalam pelayar untuk ujian asas. Sesetengah ciri PWA/offline memerlukan HTTPS atau localhost.
3. Untuk pemasangan ke skrin utama iPhone, hoskan fail ini pada laman HTTPS. Contohnya GitHub Pages atau perkhidmatan hosting statik pilihan anda.
4. Pada iPhone, buka URL HTTPS itu dalam Safari → butang Share → Add to Home Screen → Add.
5. Buka aplikasi dari ikon skrin utama dan uji tambah/edit/padam rekod.

## Import
- JSON: pilih `contoh-jadual.json` atau fail yang dieksport daripada aplikasi.
- CSV: gunakan pengepala `day,start,end,className,subject,location,alarmMinutes,alarmEnabled`.
- Fail Excel `.xlsx` tidak dibaca terus. Simpan helaian Excel sebagai CSV UTF-8 terlebih dahulu.
- Gambar/PDF: OCR/AI untuk menukarkan jadual kepada JSON belum disambungkan dalam prototaip ini. Minta ChatGPT menukarkan jadual dalam gambar/PDF kepada JSON mengikut medan di atas, semak hasilnya, simpan sebagai `.json`, kemudian import.

## Batasan penting
- Data disimpan pada LocalStorage pelayar/peranti, bukan pangkalan data awan; tidak disegerakkan antara peranti.
- Tiada login atau kawalan akses.
- Tetapan peringatan hanya disimpan sebagai data. Notifikasi/alarm sebenar belum dilaksanakan.
- Prototaip bukan aplikasi rasmi KPM.
- Buat eksport JSON secara berkala untuk sandaran.
