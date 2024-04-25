# Capstone Project Module 2 - Di Balik Kelalaian Tap Out: Identifikasi Pemicu di Halte TransJakarta

![header](doc/header.png)

## Context
Penelitian ini fokus pada ketidakpatuhan pengguna dalam sistem tap in-tap out pada TransJakarta. Meskipun kebijakan ini bertujuan menciptakan sistem pembayaran yang adil dan akurat, tapi menghadapi kendala seperti pemblokiran kartu. Tujuannya adalah mengidentifikasi faktor pemicu ketidakpatuhan tap out, khususnya di halte-halte dengan volume tinggi, untuk meningkatkan efisiensi layanan.

## Problem Statement
Penelitian bertujuan menyelidiki faktor-faktor yang berpotensi mempengaruhi ketidakpatuhan tap out di BRT TransJakarta. Rumusan masalah mencakup signifikansi masalah kepatuhan tap out, dampaknya terhadap pengguna dan pendapatan TransJakarta, identifikasi halte dengan kepadatan tertinggi, serta pemahaman faktor yang memengaruhi ketidakpatuhan.

## Data
Menggunakan dataset `Transjakarta.csv` bulan April 2023. [Download di sini](https://drive.google.com/drive/folders/1S04hk5uHfHYe6J1S6fVqDunuja1Lk1Lo)

**Deskripsi Kolom**:

| Nama Kolom        | Deskripsi                                                                                         |
|-------------------|--------------------------------------------------------------------------------------------------|
| transID           | ID transaksi yang unik untuk setiap transaksi.                                                    |
| payCardID         | Identifikasi utama dari pelanggan. Kartu yang digunakan pelanggan sebagai tiket untuk masuk dan keluar. |
| payCardBank       | Nama bank penerbit kartu pembayaran milik pelanggan.                                             |
| payCardName       | Nama pelanggan yang ada di kartu.                                                                 |
| payCardSex        | Jenis kelamin pelanggan yang ada di kartu.                                                        |
| payCardBirthDate  | Tahun kelahiran pelanggan.                                                                        |
| corridorID        | ID Koridor / ID Rute sebagai kunci untuk pengelompokan rute.                                     |
| corridorName      | Nama Koridor / Nama Rute berisi Mulai dan Selesai untuk setiap rute.                              |
| direction         | Arah rute. 0 untuk Pergi, 1 untuk Pulang.                                                         |
| tapInStops        | ID halte tempat pelanggan melakukan Tap Masuk.                                                     |
| tapInStopsName    | Nama halte tempat pelanggan melakukan Tap Masuk.                                                   |
| tapInStopsLat     | Garis lintang dari halte tempat pelanggan melakukan Tap Masuk.                                    |
| tapInStopsLon     | Garis bujur dari halte tempat pelanggan melakukan Tap Masuk.                                       |
| stopStartSeq      | Posisi halte awal dalam rute perjalanan pelanggan pada saat melakukan Tap Masuk.                   |
| tapInTime         | Waktu pelanggan melakukan Tap Masuk yang mencakup tanggal dan jam.                                 |
| tapOutStops       | ID halte tempat pelanggan melakukan Tap Keluar.                                                    |
| tapOutStopsName   | Nama halte tempat pelanggan melakukan Tap Keluar.                                                  |
| tapOutStopsLat    | Garis lintang dari halte tempat pelanggan melakukan Tap Keluar.                                     |
| tapOutStopsLon    | Garis bujur dari halte tempat pelanggan melakukan Tap Keluar.                                       |
| stopEndSeq        | Posisi halte akhir dalam rute perjalanan pelanggan pada saat melakukan Tap Keluar.                 |
| tapOutTime        | Waktu pelanggan melakukan Tap Keluar.                                                              |


## Analisis
Lihat file ipynb & ppt.

## Kesimpulan
1. **Signifikansi Masalah Kepatuhan Tap Out**: Tingkat ketidakpatuhan 3.55% berdampak pada efisiensi dan kepuasan pengguna.

2. **Dampak Ketidakpatuhan**: Kerugian finansial bagi pengguna dan pendapatan TransJakarta.

3. **Identifikasi Halte dengan Kepadatan Tertinggi**: BKN, Penjaringan, Terminal Senen, Monas, dan Terminal Kampung Rambutan.

4. **Faktor-faktor yang Berpotensi Mempengaruhi Ketidakpatuhan**: Pola Jam dan Hari Penggunaan, Jenis Kelamin Pengguna, Usia Pengguna, Kartu Pembayaran.

## Rekomendasi
1. Perkenalkan lebih banyak opsi pembayaran.
2. Tambah mesin tap out di halte padat.
3. Lakukan program pelatihan dan kampanye sosialisasi.
4. Implementasikan sistem pemantauan real-time.
5. Tambah pencahayaan dan keamanan di halte.
6. Buka kanal feedback dari pengguna.

[**Dashboard**](https://public.tableau.com/app/profile/kristian.brilyawan/viz/AnalisisKepatuhanTransJakarta/OverviewKepatuhandanDemografiPengguna#1)