# Analisis Harga Saham dengan Tableau — EA Stock Price

![Tableau](https://img.shields.io/badge/-Tableau-085041?style=flat&labelColor=E1F5EE&color=085041) ![Data Visualization](https://img.shields.io/badge/-Data%20Visualization-085041?style=flat&labelColor=E1F5EE&color=085041) ![Calculated Field](https://img.shields.io/badge/-Calculated%20Field-085041?style=flat&labelColor=E1F5EE&color=085041) ![Stock Analysis](https://img.shields.io/badge/-Stock%20Analysis-085041?style=flat&labelColor=E1F5EE&color=085041) 

---


## Tentang proyek

Proyek ini memvisualisasikan data harga saham historis menggunakan Tableau. Dataset mencakup data harga saham dari tahun 1999 hingga 2021, dengan fokus pada rata-rata harga tertinggi per tahun dan kategorisasi performa penjualan.


## Tujuan analisis

- Menampilkan tren rata-rata harga tertinggi saham dari tahun ke tahun
- Membuat kategori performa penjualan menggunakan Calculated Field
- Membandingkan nilai High Price aktual vs rata-rata penjualan tertinggi

## Dataset

Sumber: EA_stock_price.csv — 26 baris × 6 kolom

- Kolom: Date, Close Price, High Price, Low Price, Open Price, Volume
- Rentang waktu: 1999 – 2021

## Visualisasi yang dibuat


### 1. Rata-rata harga tertinggi per tahun

Bar chart horizontal menampilkan AVG(High Price) per tahun. Terlihat puncak harga tertinggi terjadi sekitar tahun 2019–2021.


### 2. Calculated field — kategori penjualan

```
// Rumus Calculated Field di Tableau:
IF AVG([High Price]) > 70
THEN "Paling Tinggi"
ELSE "Standar"
END
```


### 3. Perbandingan High Price vs rata-rata

Bar chart dengan dua layer warna membandingkan SUM(High Price) aktual dengan AGG(Rata-Rata Penjualan Tertinggi).

> Insight: Harga saham mengalami penurunan signifikan pada 2008–2012, lalu kembali meningkat dan mencapai puncak di 2020–2021.


## Tools

![Tableau Public](https://img.shields.io/badge/-Tableau%20Public-085041?style=flat&labelColor=E1F5EE&color=085041) ![Microsoft Excel](https://img.shields.io/badge/-Microsoft%20Excel-085041?style=flat&labelColor=E1F5EE&color=085041) 


## Cara melihat dashboard

Dashboard dapat diakses melalui Tableau Public di:

