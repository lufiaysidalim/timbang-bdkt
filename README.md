# Game Pengemasan BDKT

Game edukasi di peramban untuk berlatih menakar dan menimbang isi kemasan sesuai label (BDKT, Barang Dalam Keadaan Terbungkus). Pemain mengisi kemasan dengan produk sampai jumlah isi, berat bersih, bobot tuntas, atau isi bersih (mL) tepat sesuai label, sambil menjaga kepercayaan pelanggan dan kas usaha.

Satu file saja (`index.html`), tanpa instalasi, tanpa server, dan bisa dimainkan di komputer maupun ponsel.

## Cara memainkan

Buka `index.html` di peramban, atau gunakan tautan GitHub Pages repositori ini.

- **Mulai Main**: permainan penuh 100 level dengan pangkat dari Karyawan Magang sampai CEO.
- **Latihan Dahulu**: empat latihan tanpa skor, kas, dan kepercayaan, boleh diulang sebanyak mungkin, dengan waktu 150% dari waktu normal dan penjelasan cara bermain sebelum mulai. Pilih dengan tombol angka:
  1. Menakar Jumlah Isi: permen buah, 2 sampai 8 butir.
  2. Menimbang Berat Bersih: tepung terigu, 10 sampai 40 g.
  3. Menimbang Bobot Tuntas: jamur kancing, berat bersih 10 sampai 40 g.
  4. Menimbang Isi Bersih: air mineral (massa jenis 1,1 g/mL), 10 sampai 40 mL.

### Aturan singkat

- Isi kemasan sampai isinya sama dengan label, lalu tekan **Kemas**.
- **Kurang**: kepercayaan turun 2x persen kekurangan (maksimal 20%).
- **Berlebih**: kepercayaan naik 0,5x persen kelebihan (maksimal 5%), tetapi untung berkurang. Lebih dari 10% menjadi kerugian kas.
- **Waktu habis**: kemasan kosong, kepercayaan turun 20% tanpa kerugian kas. Kemasan sudah berisi tetapi belum dikemas, kepercayaan turun 25% dan kas berkurang sebesar nilai produk di kemasan.
- **Salah cairan**: Tuang Cairan pada produk selain bobot tuntas membuat isi terkontaminasi.
- **Bobot tuntas**: kelebihan cairan pengisi dihargai Rp 5 per gram dan mengurangi untung, bahkan bisa merugikan kas.
- **Mode Latihan**: tidak ada produk tumpah, hanya informasi bahwa menimbang berlebih mengurangi untung di permainan utama.
- Mulai level 61 kemasan bisa bocor, mulai level 66 isi berlebih bisa tumpah, dan mulai level 76 cairan tertentu merusak timbangan.
- **Kalah** jika kepercayaan 0%, kas negatif 5 level berturut-turut, atau level 100 selesai dengan kas negatif.
- **Menang** jika level 100 selesai dengan kas positif.

Penjelasan lengkap dengan gambar ada di menu **Informasi** di dalam game (tombol `K`).

## Pintasan keyboard

| Tombol | Fungsi |
|---|---|
| `Space` | Tuang Produk (tahan) |
| `Shift` | Tuang Cairan (mulai level 46) |
| `Enter` | Kemas, lanjut, atau mulai |
| `Backspace` | Kurangi |
| `Y` | Ganti kemasan (1x per level, kecuali kemasan bocor) |
| `T` | Tare |
| `1` `2` `3` | Pakai bantuan: Target Menimbang, Tambahan Waktu 2x, Perisai Pengaman |
| `Q` `W` `E` | Beli bantuan |
| `Esc` | Jeda, atau batal di dialog |
| `J` | Restart level |
| `Del` | Reset dari awal |
| `L` | Pilih level (perlu password) |
| `K` | Informasi (slide: panah kiri dan kanan, `Esc` keluar) |
| `Home` | Kembali ke menu awal (konfirmasi: `Enter` = Ya, `Space` = Tidak) |
| `I` `O` `P` | Suara, Getar, Efek |

Di layar sentuh: tekan dan tahan kemasan untuk menuang, ketuk dua kali untuk ganti produk atau cairan, geser atas untuk Tare, kiri untuk Kurangi, bawah untuk Ganti, dan kanan untuk Kemas.

## Memasang di GitHub Pages

1. Unggah `index.html` ke root repositori (bukan di dalam folder).
2. Buka **Settings > Pages**.
3. Pada **Build and deployment**, pilih **Deploy from a branch**, lalu branch `main` dan folder `/ (root)`.
4. Tunggu beberapa menit. Game bisa dimainkan di `https://NAMAAKUN.github.io/NAMAREPO/`.

Semua gambar sudah tertanam di dalam `index.html`, jadi tidak ada berkas lain yang perlu diunggah. Skor terbaik tiap pemain disimpan di peramban masing-masing (`localStorage`).

## Catatan

- Versi: beta-mild 231126.
- Seluruh grafik dibuat sebagai SVG, sehingga tajam di semua ukuran layar.
- Game ini untuk pembelajaran dan hiburan. Angka harga dan biaya di dalam game hanya contoh dan bukan acuan resmi.
