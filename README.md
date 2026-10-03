# Analisis_Volume_Lambung_Kapal

# Perhitungan Volume Lambung Kapal

Program ini digunakan untuk menghitung volume kedua lambung kapal menggunakan metode **Trapesium** dan **Simpson 1/3**.

##  Tujuan

Menghitung dan membandingkan volume kedua lambung kapal menggunakan integrasi numerik.

##  Metode

Jarak antar stasiun:

$$ \Delta x = 10 \text{ cm} $$


Luas penampang:

$$ A = \text{lebar} \times \text{tinggi} $$


Volume satu lambung dihitung dengan:

**Trapesium**
$$ V = h \left[ \frac{A_0 + A_n}{2} + \sum A_i \right] $$

**Simpson 1/3**
$$ V = \frac{h}{3} \left[ A_0 + A_n + 4 \sum A_{\text{ganjil}} + 2 \sum A_{\text{genap}} \right] $$


Hasil volume satu lambung kemudian dikalikan 2 karena terdapat dua lambung.

##  Flowchart

```text
Data Penampang
      ↓
Δx = 10 cm
      ↓
Hitung Luas Penampang
      ↓
Trapesium & Simpson 1/3
      ↓
Volume 1 Lambung
      ↓
× 2 Lambung
      ↓
Perbandingan Hasil
