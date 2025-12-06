# Angkot Bandung Mapping – Database & Geospatial Processing

Berfokus pada pengolahan data trayek angkot Kota Bandung untuk periode 2003–2018. Proses mencakup data cleaning, import, serta analisis spatial menggunakan PostGIS.

## Detail

### 1. Pengolahan Data Armada dan Trayek
- Menggabungkan data armada per tahun ke dalam satu set terstruktur.
- Melakukan preprocessing untuk menyatukan data 2003–2018.
- Mengekspor data ke CSV dan import ke DBeaver.

### 2. Import Data Geometri Rute Angkot
- Mengimport data rute dalam format CSV berisi geometri.
- Melakukan pengecekan struktur dan validasi geometri sebelum dimasukkan ke database.

### 3. Impor Data Kelurahan Bandung
- Mengambil data geoJSON kelurahan.
- Mengonversi dan mengimpor menggunakan QGIS (ogr2ogr).
- Memastikan data spatial tampil dan terbaca dengan benar.

### 4. Analisis Spasial (PostGIS)
- Menghitung jumlah trayek angkot per tahun.
- Menghitung total armada angkot per tahun.
- Menghitung total armada yang melintasi tiap kelurahan.

## Output
- Tabel rangkuman trayek 2003–2018.
- Tabel total armada per tahun.
- Tabel interseksi trayek dan kelurahan berbasis buffer.
- Tabel akumulasi armada per kelurahan.
