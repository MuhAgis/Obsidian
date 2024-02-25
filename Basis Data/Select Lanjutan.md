# AND 
## Struktur
```sql
select * from nama_table where kolom1="nilai_kolom1" AND kolom2="nama_kolom2";
```
## Contoh
```sql
select * from mobil where warna="Hitam" AND pemilik="Ibrahim";
```
## Hasil
![a](asett/and.png)
## Analisis
## Kesimpulan
# OR
## Struktur 
```sql
select * from nama_table where kolom1="nilai_kolom1" OR kolom2="nilai_kolom2";
```
## Contoh 
```sql
select * from mobil where warna="Hitam" OR pemilik="Ibrahim";
```
## Hasil
![a](asett/or.png)
## Analisis
## Kesimpulan 
# Between
## Struktur
```sql
select * from nama_table where nama_kolom between nilai1 AND nilai2;
```
## Contoh
```sql
select * from mobil where harga_rental between 100000 AND 150000;
```
## Hasil
![a](asett/between.png)
## Analisis
## Kesimpulan
# Not Between
## Struktur
```sql
select * from nama_table where nama_kolom Not between nilai1 AND nilai2;
```
## Contoh
```sql
select * from mobil where harga_rental not between 100000 AND 150000;
```
## Hasil
![a](asett/nbetween.png)
## Analisis 
## Kesimpulan 
# <=
## Struktur
```sql
SELECT * FROM nama_table WHERE nama_kolom <= nilai;
```
## Contoh
```sql
SELECT * FROM mobil WHERE harga_rental <= 50000;
```
## Hasil
![a](asett/kecil.png)
## Analisis 
## Kesimpulan 
# >=
## Struktur
```sql
SELECT * FROM nama_table WHERE nama_kolom >= nilai;
```
## Contoh
```sql
SELECT * FROM mobil WHERE harga_rental >= 50000;
```
## Hasil
![a](asett/besar.png)
## Analisis 
## Kesimpulan 
# <> atau !=
## Struktur
```sql
select * from nama_table where nama_kolom <> 50000;
```
## Contoh
```sql
select * from mobil where harga_rental <> 50000;
```
## Hasil
![a](asett/kecil_besar.png)
## Analisis 
## Kesimpulan 
# Tantangan 
## Struktur
```sql
select nama_kolom from nama_table where nama_kolom="nilai_kolom";
```
## Contoh
```sql
select pemilik from mobil where no_plat="DD 2650 XY";
```
## Hasil
![a](asett/tantangan.png)
## Analisis 
## Kesimpulan 