Perhitungan Volume Lambung Kapal Menggunakan Metode Numerik

Deskripsi Proyek

Proyek ini bertujuan untuk memperkirakan volume lambung kapal menggunakan metode integrasi numerik, yaitu Metode Trapesium dan Metode Simpson 1/3. Perhitungan dilakukan berdasarkan gambar kapal yang dibagi menjadi beberapa stasiun untuk memperoleh data luas penampang sepanjang lambung kapal.

Ukuran satu kotak pada gambar ditetapkan sebesar 45 cm. Data dimensi tersebut digunakan untuk menentukan luas penampang pada setiap stasiun, yang selanjutnya diintegrasikan secara numerik untuk memperoleh estimasi volume lambung kapal.

Tujuan

Menghitung estimasi volume lambung kapal berdasarkan data penampang.

Menerapkan metode Trapesium dan Simpson 1/3 dalam integrasi numerik.

Membandingkan hasil estimasi volume dari kedua metode.

Memvisualisasikan perubahan luas penampang sepanjang lambung kapal menggunakan Python.

Ketentuan dan Asumsi

Ukuran satu kotak pada gambar kapal adalah 45 cm atau 0,45 meter.

Lambung kapal dibagi menjadi beberapa stasiun pengamatan.

Luas penampang dihitung menggunakan pendekatan lebar dikalikan tinggi, dengan asumsi lantai kapal datar dan tanpa keel.

Volume reserve buoyancy tidak diperhitungkan.

Kapal memiliki dua lambung yang diasumsikan memiliki bentuk dan ukuran yang sama.

Hasil perhitungan merupakan estimasi numerik berdasarkan data dan asumsi yang digunakan.

Metode Perhitungan

1. Menentukan Luas Penampang

Luas penampang pada setiap stasiun dihitung menggunakan pendekatan:

[
A_i = \text{lebar}_i \times \text{tinggi}_i
]

Keterangan:

(A_i) adalah luas penampang pada stasiun ke-(i).

Lebar dan tinggi merupakan dimensi lambung kapal pada stasiun tersebut.

2. Metode Trapesium

Metode Trapesium digunakan untuk memperkirakan volume berdasarkan luas penampang pada stasiun yang berurutan.

[
V \approx h\left[\frac{A_0+A_n}{2}+\sum_{i=1}^{n-1}A_i\right]
]

Metode ini menghitung pendekatan volume dengan membagi lambung kapal menjadi beberapa bagian berbentuk trapesium.

3. Metode Simpson 1/3

Metode Simpson 1/3 menggunakan pendekatan parabola untuk memperkirakan integral numerik.

[
V \approx \frac{h}{3}\left[A_0+A_n+
4\sum A_{\text{ganjil}}+
2\sum A_{\text{genap}}\right]
]

Metode ini mensyaratkan jumlah interval yang genap agar dapat diterapkan pada keseluruhan rentang pengamatan.

4. Menghitung Volume Total

Jika kedua lambung kapal dianggap identik, volume total dihitung dengan:

[
V_{\text{total}}=2V_{\text{satu lambung}}
]

Konversi dari cm³ ke liter dilakukan dengan membagi nilai volume dengan 1.000.

Hasil Perhitungan

Berdasarkan hasil perhitungan pada notebook, diperoleh estimasi berikut:

Metode

Volume Total

Trapesium

14.106,15 liter

Simpson 1/3

14.147,46 liter

Selisih hasil kedua metode adalah 41,31 liter. Perbedaan ini terjadi karena masing-masing metode menggunakan pendekatan numerik yang berbeda dalam memperkirakan volume.

Catatan: Nilai tersebut merupakan hasil yang dilaporkan oleh notebook dan perlu diverifikasi terhadap data penampang serta implementasi kode sebelum digunakan sebagai hasil akhir penelitian.

Visualisasi

Proyek ini menggunakan visualisasi untuk membantu memahami:

Perubahan luas penampang pada setiap stasiun.

Pendekatan integrasi menggunakan metode Trapesium.

Pendekatan integrasi menggunakan metode Simpson 1/3.

Perbandingan estimasi volume dari kedua metode.

Tools dan Teknologi

Python — bahasa pemrograman untuk perhitungan numerik.

Google Colab / Jupyter Notebook — lingkungan untuk menjalankan kode.

NumPy — pengolahan data numerik.

Matplotlib — pembuatan grafik dan visualisasi.

Cara Menjalankan Proyek

Unduh atau clone repository ini.

Buka file notebook .ipynb menggunakan Google Colab atau Jupyter Notebook.

Pastikan pustaka Python yang diperlukan telah tersedia.

Jalankan setiap sel kode secara berurutan.

Periksa hasil perhitungan dan visualisasi yang dihasilkan.

Kesimpulan

Perhitungan volume lambung kapal dapat dilakukan menggunakan metode Trapesium dan Simpson 1/3 berdasarkan data luas penampang pada setiap stasiun. Kedua metode menghasilkan estimasi volume yang dapat dibandingkan untuk mengevaluasi hasil integrasi numerik.

Keakuratan hasil bergantung pada ketepatan pengukuran gambar, konsistensi satuan, data luas penampang, dan penerapan rumus pada program.

Identitas

Nama: Muhammad Wildan Zahir

NPM: 25083010002

Mata Kuliah: Analisis Numerik
