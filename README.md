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
- **Bobot tuntas**: untung = 10% x nilai bobot tuntas (hanya produk utama, bukan 10% x berat bersih). Kelebihan cairan pengisi dihargai Rp 20 per gram dan mengurangi untung. Kelebihan produk utama (jamur, buah, sarden) tetap mengurangi untung sesuai harga produknya, dan bila lebih dari bobot tuntas +10% untung habis dan kas berkurang. Sebelum level 66 belum ada aturan tumpah, jadi kelebihan bisa sangat banyak sampai merugikan kas.
- **Mode Latihan**: tidak ada produk tumpah, hanya informasi bahwa menimbang berlebih mengurangi untung di permainan utama.
- **Kuis pelabelan**: waktu menjawab 6 sampai 12 detik, menyesuaikan panjang soal dan pilihan jawaban.
- **Tinggi isi sebanding berat**: kemasan penuh berarti isi mencapai ujung atas bagian bening (tepi jendela, bibir kaleng, atau leher botol), yaitu berat label +10% (minimal +1 g). Mulai level 66, isi sampai titik itu tumpah.
- Mulai level 61 kemasan bisa bocor (baru ketahuan setelah diisi), mulai level 66 isi berlebih bisa tumpah, dan mulai level 76 cairan tertentu merusak timbangan.
- **Kerusakan timbangan** (bocor = 50% dari biaya tumpah):

| Cairan | Bocor | Tumpah |
|---|---|---|
| Kecap (Lv 76) | Rusak ringan, Rp 1.500 | Rusak ringan, Rp 3.000 |
| Minyak (Lv 86) | Rusak ringan, Rp 2.500 | Rusak berat, Rp 5.000 |
| Air mineral (Lv 96) | Rusak berat, Rp 5.000 | Rusak fatal, Rp 10.000 |

  Bocor atau tumpah produk padat Rp 500 dan cairan lain Rp 1.000. Saat kejadian muncul kartu keterangan beserta ikon kerusakan, dan seluruh kotak area permainan berkedip transparan sebagai peringatan (ikut pengaturan Efek, tombol `P`).
- **Kalah** jika kepercayaan 0%, kas negatif 5 level berturut-turut, atau level 100 selesai dengan kas negatif.
- **Menang** jika level 100 selesai dengan kas positif.

Penjelasan lengkap dengan gambar ada di menu **Informasi** di dalam game (tombol `K`).

## Bentuk kemasan

Setiap produk punya bentuk kemasan sendiri, tetap dengan bagian bening untuk melihat isi, merek, keterangan kuantitas, angka, dan satuan. Ukuran kemasan menyesuaikan label (jumlah isi, berat bersih, bobot tuntas, atau isi bersih): label kecil = kemasan kecil, label besar = kemasan besar, tetapi selalu muat di antara corong dan timbangan. Ukuran butiran produk tetap untuk tiap produk dan jenis takaran, sama dengan butiran di corong dan yang masuk ke kemasan. Kemasan penuh tepat pada label +10%. Kaca pembesar memperbesar keterangan pada label.

| Produk | Kemasan |
|---|---|
| Permen buah | Kantong permen kenyal bergigi segel |
| Wafer vanila | Bungkus flow-pack dengan ujung bergerigi |
| Coklat bar | Bar berbungkus foil ungu |
| Keripik ubi | Pouch berdiri premium dengan zipper |
| Kacang oven | Toples bening bertutup merah |
| Tepung terigu | Kantong kertas berjendela plastik |
| Jamur kancing | Pouch bening dengan kartu header |
| Potongan buah | Kaleng tinggi |
| Ikan sarden | Kaleng sarden lebar dengan cincin tarik |
| Kecap manis | Botol plastik bahu lebar |
| Minyak sawit | Botol minyak bergagang |
| Air mineral | Botol PET bergelombang |

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
