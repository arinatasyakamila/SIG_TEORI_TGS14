# SIG_TEORI_TGS14
 Searching and Downloading OpenStreetMap Data
# Langkah Kerja :

1. Cari dan pasang plugin QuickOSM dari QGIS Official Plugin Repository. Lihat Menggunakan Plugin untuk instruksi mengunduh plugin. Pastikan Anda telah memilih kotak centang. Klik Close.

2. Setelah diinstal, luncurkan plugin dari Vector ‣ QuickOSM ‣ QuickOSM….

3. Di tab Kueri cepat, Anda dapat menyetel filter untuk memilih subkumpulan. Atribut fitur peta dalam database OSM disimpan sebagai Tag. Tag diwakili dengan kunci dan nilai. Kuncinya adalah topik dan nilai adalah bentuk spesifik. Lihat halaman wiki Fitur Peta OSM untuk daftar lengkap tag untuk berbagai jenis fitur. Bar direpresentasikan menggunakan tag amenity:bar dan pub dengan tag amenity:pub. Kami pertama-tama akan mengekstrak bilah. Pilih kemudahan sebagai Key dari menu drop-down.

4. Pilih bilah dari menu tarik-turun Value.

5. Kami dapat menghubungkan beberapa kueri dalam versi terbaru (v2.0.0 +) dari plugin QuickOSM. Klik tombol plus, bilah pemilihan kueri berikutnya akan muncul. Klik pada kotak pilihan pertama di mana kita bisa mendapatkan opsi And dan Or. And hanya akan memilih fitur yang benar untuk semua kueri. Or akan memilih semua fitur yang benar untuk salah satu kueri. Klik Or untuk memilih fitur bar dan pub.

6. Pilih kemudahan sebagai Kunci dari menu tarik-turun. Kemudian pilih pub dari menu tarik-turun Value.

7. Masukkan London sebagai In untuk membatasi pencarian di dalam batas kota.

8. Perluas bagian Advanced. Dalam model data OSM, fitur direpresentasikan menggunakan nodes, ways and relations. Karena kami tertarik dengan fitur titik, Anda hanya dapat memilih Node dan Points . Klik Run kueri.

9. Setelah kueri selesai, alihkan ke jendela utama QGIS. Anda akan melihat layer baru bernama amenity_bar_amenity_pub_London ditambahkan ke panel Layers. Kanvas akan menunjukkan lokasi bar dan pub yang diekstraksi.

10. Buka tabel Attribute pada layer. Ada 2.091 fitur. Fasilitas kolom berisi kategori apakah fitur tersebut pub atau bar. Dengan menggunakan kolom kategoris ini, mari menata layer kita.

11. Klik pada icon panel Open the Layer Styling, pilih Categorized lalu pada Value pilih amenity lalu klik Classify. Sekarang layer akan ditata dengan 2 warna yang menampilkan bar dan pub.

12. Sekarang klik kanan pada layer, Export Save Feature As… untuk mengekspor layer sebagai GeoPackage.

13. Di kotak dialog Save Vector Layer as…, di Format pilih GeoPackage, di File name klik ... dan ramban ke direktori tempat Anda ingin menyimpan data dan beri nama keluaran london.gpkg. Di Layer name masukkan bar_and_pubs. Klik OK.

14. Sekarang lapisan GeoPackage london_bar_and_pubs akan ditambahkan ke kanvas.
