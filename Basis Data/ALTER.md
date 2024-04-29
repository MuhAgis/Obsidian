# Menambahkan kolom
## Struktur
## Contoh
```sql
ALTER TABLE mobil ADD batas_pemnijaman varchar(10) AFTER peminjam;
```
## Hasil
### Before
![a](Asett/Ss1.png)
### After
![a](Asett/Ss2.png)
## Analisis
## Kesimpulan
## Tambahan
![a](Asett/Ss4.png)
# Mengubah nama kolom
## Struktur 
## Contoh
```sql
ALTER TABLE mobil RENAME COLUMN batas_pemnijaman TO deadline;
```
## Hasil
![a](Asett/Ss3.png)
## Analisis
## Kesimpulan
# Mengubah tipe data kolom
## Struktur 
## Contoh
```sql
ALTER TABLE mobil MODIFY deadline DATE;
```
## Hasil
![a](Asett/Ss5.png)
## Analisis
## Kesimpulan
# Menambahkan Constraint
## Struktur 
## Contoh
```sql
ALTER TABLE mobil
ALTER deadline SET DEFAULT 'Ready';
```
## Hasil
![a](Asett/Ss6.png)
## Analisis
## Kesimpulan
