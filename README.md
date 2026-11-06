# SPMB TP. 2027/2028 - SMPIT & SMAIT Insan Mandiri Greenville

Catatan untuk panitia/admin. Bagian "Cara membuka Ukur Seragam" paling sering dicari.

## Link yang dibagikan

Cukup bagikan **satu link menu**:

https://img-prog.github.io/Observasi-SMPIT-SMAIT-IMG/

Link langsung (opsional):
- Observasi: `.../tes-observasi.html`
- Wawancara Orang Tua: `.../wawancara-ortu.html`
- Ukur Seragam: `.../ukur-seragam.html`

## Isi repository

| File | Fungsi |
|---|---|
| `index.html` | Menu utama (tiga kartu) |
| `tes-observasi.html` | Observasi, dikerjakan murid |
| `wawancara-ortu.html` | Wawancara, diisi orang tua |
| `ukur-seragam.html` | Ukur seragam, diisi orang tua |
| `*.png` | Logo dan ikon. Jangan diganti namanya |

## Cara membuka Ukur Seragam

Menu Ukur Seragam dikunci sampai tanggal tertentu. Tanggal bukanya saat ini: **16 Maret 2027**.

**Cara 1: tunggu saja.** Pada tanggal itu menunya terbuka otomatis. Tidak perlu berbuat apa-apa.

**Cara 2: buka lebih awal atau ubah tanggalnya.** Tanggal yang sama ada di **dua file**, dan keduanya harus diubah:

1. Buka repository di GitHub, klik file `index.html`.
2. Klik ikon **pensil** (Edit this file) di kanan atas isi file.
3. Cari baris `const BUKA_UKUR_SERAGAM = '2027-03-16';` (tekan Ctrl+F).
4. Ganti tanggalnya. Formatnya `TAHUN-BULAN-TANGGAL`.
   - Mau langsung dibuka sekarang: isi tanggal hari ini atau tanggal yang sudah lewat, misalnya `2026-01-01`.
   - Mau diundur: isi tanggal yang baru.
5. Klik **Commit changes**, lalu **Commit changes** lagi di jendela konfirmasi.
6. Ulangi langkah 1 sampai 5 untuk file `ukur-seragam.html`.
7. Tunggu sekitar 1 menit, buka link menu, tekan Ctrl+F5.

Kalau hanya satu file yang diubah, hasilnya tidak sinkron (misalnya menu sudah terbuka tapi halamannya masih menolak).

**Uji coba sebelum dibuka:** buka `.../ukur-seragam.html?preview=1`

## Data masuk ke mana

Semua data masuk ke satu Google Sheets, dalam tab terpisah:
- `Rekap Observasi`
- `Wawancara Ortu`
- `Ukuran Seragam`

Tab baru dibuat otomatis saat data pertama masuk. Jangan ubah nama judul kolom di baris pertama.

## Kalau kode Google Apps Script diubah

Setelah menyimpan kode, wajib deploy ulang: **Deploy, Kelola deployment, ikon pensil, Versi baru, Deploy**. Tanpa itu perubahan tidak aktif. URL-nya tidak berubah.

## Menambah atau mengganti file di GitHub

**Add file, Upload files**, seret filenya, lalu **Commit changes**. Kalau nama file sama, file lama otomatis tertimpa. Pastikan nama tidak bertambah angka seperti `index (1).html`.
