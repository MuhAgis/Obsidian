# 14
## Query
```sql
SELECT MAX(Gaji) AS GajiTerbesar, MIN(Gaji) AS GajiTerkecil
FROM pegawai
WHERE Jabatan = "Manajer";
```
## Hasil
![](14.png)
## Analisis
- `SELECT`= Untuk memilih kolom nama mana saja yang dipilih untuk ditampilkan l.
- `MAX(Gaji)`= Untuk menampilkan nilai terbesar dari suatu data dalam kolom yang dipilih. Gaji  adalah nama kolom yang dipilih.
- `AS GajiTerbesar`= Untuk Menganti nama dari kolom hasil `MAX(Gaji)` menjadi `GajiTerbesar` untuk sementara.
- `MIN(Gaji)`= Untuk menampilkan nilai terkecil dari suatu data dalam kolom yang dipilih. Gaji adalah nama kolom yang dipilih.
- `AS GajiTerkecil`= Untuk Menganti nama dari kolom hasil `MIN(Gaji)` menjadi `GajiTerkecil` untuk sementara.
- `FROM pegawai`= Untuk memilih dari tabel mana yang data kolomnya ingin ditampilkan.
- `WHERE`= Kondisi yang harus dipenuhi oleh suatu kolom data agar bisa ditampilkan.
- `(Jabatan = "Manajer")`= Kondisi dari `WHERE` yang harus dipenuhi. Barisan data yang kolom jabatannya berisi manajer akan ditampilkan kolom Gajinya.
- **Hasilnya** = Jabatan Manajer yang memiliki nilai maksimum adalah 6250000 kolom hasil `MAX`nya diubah jadi `GajiTerbesar`.  
  Sedangkan nilai minimumnya adalah 5250000 kolom hasil `MIN`nya diubah jadi `GajiTerkecil`
# 15
## Query
```sql
SELECT NoCab, MAX(Gaji) AS GajiTerbesar, MIN(Gaji) AS GajiTerkecil
FROM pegawai
GROUP BY NoCab;
```
## Hasil
![](15.png)
## Analisis
- `SELECT`= Untuk memilih kolom nama mana saja yang dipilih untuk ditampilkan.
- `NoCab`= Nama kolom yang ingin ditampilkan.
- `MAX(Gaji)`= Untuk menampilkan nilai terbesar dari suatu data dalam kolom yang dipilih. Gaji  adalah nama kolom yang dipilih.
- `AS GajiTerbesar`= Untuk Menganti nama dari kolom hasil `MAX(Gaji)` menjadi `GajiTerbesar` untuk sementara.
- `MIN(Gaji)`= Untuk menampilkan nilai terkecil dari suatu data dalam kolom yang dipilih. Gaji adalah nama kolom yang dipilih.
- `AS GajiTerkecil`= Untuk Menganti nama dari kolom hasil `MIN(Gaji)` menjadi `GajiTerkecil` untuk sementara.
- `FROM pegawai`= Untuk memilih dari tabel mana yang data kolomnya ingin ditampilkan.
- `GROUP BY`= Untuk mengelompokkan data berdasarkan nilai data yang telah ditentukan pada kolom yang dipilih.
- `NoCab`= Nama kolom yang ingin dikelompokkan.
- **Hasilnya** = Masing-masing `NoCab` dicari nilai maksimum dan minimumnya. Mulai dari C101,C102,,C103,C104 dan nama hasil kolomnya diubah menjadi `GajiTerbesar` dan `GajiTerkecil`.
# 16
## Query
```sql
SELECT NoCab, MAX(Gaji) AS GajiTerbesar, MIN(Gaji) AS GajiTerkecil
FROM pegawai
GROUP BY NoCab HAVING COUNT(NIP) >= 3;
```
## Hasil
![](16.png)
## Analisis
- `SELECT`= Untuk memilih kolom nama mana saja yang dipilih untuk ditampilkan.
- `NoCab`= Nama kolom yang ingin ditampilkan.
- `MAX(Gaji)`= Untuk menampilkan nilai terbesar dari suatu data dalam kolom yang dipilih. Gaji  adalah nama kolom yang dipilih.
- `AS GajiTerbesar`= Untuk Menganti nama dari kolom hasil `MAX(Gaji)` menjadi `GajiTerbesar` untuk sementara.
- `MIN(Gaji)`= Untuk menampilkan nilai terkecil dari suatu data dalam kolom yang dipilih. Gaji adalah nama kolom yang dipilih.
- `AS GajiTerkecil`= Untuk Menganti nama dari kolom hasil `MIN(Gaji)` menjadi `GajiTerkecil` untuk sementara.
- `FROM pegawai`= Untuk memilih dari tabel mana yang data kolomnya ingin ditampilkan.
- `GROUP BY`= Untuk mengelompokkan data berdasarkan nilai data yang telah ditentukan pada kolom yang dipilih.
- `NoCab`= Nama kolom yang ingin dikelompokkan.
- `HAVING`= Kondisi yang harus dipenuhi oleh suatu kelompok data.
- `(COUNT(NIP) >= 3`= Kondisi dari `HAVING` hanya hasil hitung kolom `NIP` yang lebih dari atau sama dengan 3 yang muncul.
- **Hasilnya** = Seperti no.4, yang mempunyai hasil hitung lebih dari atau sama dengan 3 adalah `NoCab C102`. Jadi hanya itu yang dicari nilai maksimum dan minimumnya pada kolom `Gaji`.