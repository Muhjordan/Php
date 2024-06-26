# AND
## Struktur Query
```Sql
SELECT warna,pemilik FROM mobil WHERE warna="Hitam" AND pemilik="Ibrahim";
```
## Contoh Query 
```sql
SELECT warna,pemilik FROM mobil WHERE warna="Hitam" AND pemilik="Jordan";
```
## Hasil Program
![gambar](Aset/IMG_1.jpg)

## Analisis
`SELECT warna, pemilik`: Pernyataan SELECT ini menentukan kolom-kolom mana yang akan diambil dari tabel "mobil", yaitu kolom "warna" dan "pemilik".

`FROM mobil`: Mengidentifikasi tabel yang akan digunakan dalam operasi SELECT, yaitu tabel "mobil".

`WHERE warna="Hitam" AND pemilik="Jordan"`: Klausul WHERE digunakan untuk menerapkan kriteria seleksi pada data yang akan diambil. Dalam hal ini, hanya data yang memiliki nilai "warna" sama dengan "Hitam" dan nilai "pemilik" sama dengan "Jordan" yang akan dipilih
## Kesimpulan 
pernyataan SELECT ini akan mengambil data warna dan pemilik dari tabel "mobil" yang memiliki warna "Hitam" dan pemilik "Jordan".
# OR
## Struktur Query
```sql
SELECT warna,pemilik FROM mobil WHERE warna="Hitam" OR pemilik="Ibrahim";
```
## Contoh Query
```sql
select warna,pemilik from mobil where warna="Hitam" OR pemilik="Jordan";
```
## Hasil Program
![gambar](Aset/IMG_2.jpg)

## Analisis
`SELECT warna, pemilik`: Pernyataan SELECT menentukan kolom mana yang akan diambil dari tabel "mobil", yaitu kolom "warna" dan "pemilik".

`FROM mobil`: Mengidentifikasi tabel yang akan digunakan dalam operasi SELECT, yaitu tabel "mobil".

`WHERE warna="Hitam" OR pemilik="Jordan"`: Klausul WHERE digunakan untuk menerapkan kriteria seleksi pada data yang akan diambil. Dalam hal ini, data akan dipilih jika memiliki nilai "warna" sama dengan "Hitam" atau nilai "pemilik" sama dengan "Jordan".
## Kesimpulan 
pernyataan SELECT ini akan mengambil data warna dan pemilik dari tabel "mobil" yang memiliki warna "Hitam" atau pemilik "Jordan".
# BETWEEN
## Struktur Query
```sql
SELECT * FROM mobil WHERE harga_rental BETWEEN 100000 AND 200000;
```
## Contoh Query 
```SQL
select * from mobil where harga_rental BETWEEN 100000 AND 150000;
```
## Hasil Program
![gambar](Aset/IMG_3.jpg)

## Analisis
`SELECT` : Pernyataan SELECT ini menunjukkan bahwa kita akan mengambil semua kolom dari tabel "mobil".

`FROM mobil`: Mengidentifikasi tabel yang akan digunakan dalam operasi SELECT, yaitu tabel "mobil".

`WHERE harga_rental BETWEEN 100000 AND 150000`: Klausul WHERE digunakan untuk menerapkan kriteria seleksi pada data yang akan diambil. Dalam hal ini itu harga_rental" dalam rentang antara 100.000 dan 150.000.
# NOTWEEN
## Struktur Query
```sql
SELECT * FROM mobil WHERE harga_rental NOT BETWEEN 100000 AND 200000;
```
## Contoh Query 
```SQL
select * from mobil where harga_rental NOT BETWEEN 100000 AND 150000;
```
## Hasil Program

![gambar](Aset/IMG_4.jpg)

## Analisis
`SELECT` : Pernyataan SELECT ini menunjukkan bahwa kita akan mengambil semua kolom dari tabel "mobil".

`FROM mobil`: Mengidentifikasi tabel yang akan digunakan dalam operasi SELECT, yaitu tabel "mobil".

`WHERE harga_rental NOT BETWEEN 100000 AND 150000`: Klausul WHERE digunakan untuk menerapkan kriteria seleksi pada data yang akan diambil. Dalam hal ini, data akan dipilih jika nilai "harga_rental" tidak berada dalam rentang antara 100.000 dan 150.000.
## Kesimpulan 
pernyataan SELECT ini akan mengambil semua kolom dari tabel "mobil" untuk data yang memiliki nilai "harga_rental" di luar rentang antara 100.000 dan 150.000.
# <=
## Struktur Query
```sql
SELECT FROM * mobil WHERE harga_rental <= 50000;
```
## Contoh Query 
```sql
select * from mobil where harga_rental <= 100000;
```
## Hasil Program
![gambar](Aset/IMG_5.jpg)

## Analisis
`SELECT` : Pernyataan SELECT ini menunjukkan bahwa kita akan mengambil semua kolom dari tabel "mobil".

`FROM mobil`: Mengidentifikasi tabel yang akan digunakan dalam operasi SELECT, yaitu tabel "mobil".

`WHERE harga_rental <= 100000`: Klausul WHERE digunakan untuk menerapkan kriteria seleksi pada data yang akan diambil. Dalam hal ini, data akan dipilih jika nilai "harga_rental" kurang dari atau sama dengan 100.000.
## Kesimpulan 
pernyataan SELECT ini akan mengambil semua kolom dari tabel "mobil" untuk data yang memiliki nilai "harga_rental" kurang dari atau sama dengan 100.000.
# >=
## Struktur Query
```sql
SELECT FROM * mobil WHERE harga_rental >= 50000;
```
## Contoh Query 
```sql
select * from mobil where harga_rental >= 100000;
```
## Hasil Program
![gambar](Aset/IMG_6.jpg)

## Analisis
`SELECT` : Pernyataan SELECT ini menunjukkan bahwa kita akan mengambil semua kolom dari tabel "mobil".

`FROM mobil`: Mengidentifikasi tabel yang akan digunakan dalam operasi SELECT, yaitu tabel "mobil".

`WHERE harga_rental >= 100000`: Klausul WHERE digunakan untuk menerapkan kriteria seleksi pada data yang akan diambil. Dalam hal ini, data akan dipilih jika nilai "harga_rental" lebih besar dari atau sama dengan 100.000.
## Kesimpulan 
pernyataan SELECT ini akan mengambil semua kolom dari tabel "mobil" untuk data yang memiliki nilai "harga_rental" lebih besar dari atau sama dengan 100.000.
# <> atau !=
## Struktur Query
```sql
SELECT FROM * mobil WHERE harga_rental <> 50000;
```
## Contoh Query 
```sql
select * from mobil where harga_rental <> 100000;
```
## Hasil Program

![gambar](Aset/IMG_7.jpg)

## Analisis 
`SELECT` : Ini menunjukkan bahwa kita ingin mengambil semua kolom dari tabel "mobil".
`FROM mobil`: Menunjukkan bahwa kita ingin mengambil data dari tabel "mobil".
`WHERE harga_rental <> 100000`: Ini adalah klausa WHERE yang memfilter data, hanya mengambil baris di mana nilai kolom "harga_rental" tidak sama dengan 100.000.
## Kesimpulan 
semua kolom data dari tabel "mobil" dimana nilai kolom "harga_rental" tidak sama dengan 100.000.

Hasilnya akan mencantumkan semua data mobil yang harga rentalnya berbeda dari 100.000, sehingga akan mencakup semua harga rental kecuali 100.000.
# Tantangan

## Struktur Query
```sql
Select kondisi from nama_tabel where kondisi="":
```

## Contoh Query 
```sql
Select kondisi from mobil where warna="Biru":
```
## Hasil Program
![](Aset/IMG_8.jpg)

## Analisis 
`SELECT kondisi`: Menunjukkan bahwa hanya nilai dari kolom "kondisi" yang akan diambil.
`FROM mobil`: Menunjukkan bahwa pengambilan data dilakukan dari tabel "mobil".
`WHERE warna = "Biru"`: Ini adalah klausa WHERE yang berfungsi sebagai filter untuk memilih baris yang memiliki nilai "Biru" di kolom "warna".
## Kesimpulan 
mengambil nilai dari kolom "kondisi" dari tabel "mobil" dimana nilai kolom "warna" adalah "Biru".

Hasilnya akan mencantumkan nilai dari kolom "kondisi" untuk setiap baris yang memiliki nilai "Biru" di kolom "warna" dalam tabel "mobil".
# IN
## Struktur Query
```sql
select * from nama_tabel where data IN('nilai 1','nilai 2');
```
## Contoh Query
```sql
select * from mobil where warna IN('pink','biru');
```
## Hasil
![gambar](Aset/IMG_9.jpg)

## Analisis
`SELECT` : Ini menunjukkan bahwa kita ingin mengambil semua kolom dari tabel "mobil".
`FROM mobil`: Menunjukkan bahwa kita ingin mengambil data dari tabel "mobil".
`WHERE warna IN ('pink', 'biru')`: Ini adalah klausa WHERE yang memfilter data, hanya mengambil baris di mana nilai kolom "warna" adalah 'pink' atau 'biru'.
Hasilnya akan mencakup semua data mobil dengan warna 'pink' atau 'biru'.
## Kesimpulan 
pernyataan SELECT ini akan mengambil semua kolom dari tabel "mobil" untuk data yang memiliki nilai "warna" sama dengan 'pink' atau 'biru'.
# IN/AND
## Struktur
```sql
select * from nama_tabel where data IN('nilai 1','nilai 2')AND data 2=nilai 1;
```
## Contoh Query
```sql
select * from mobil where warna IN('pink','biru')AND harga_rental=50000;
```
## Hasil
![gambar](IMG_10.jpg)


## Analisis
`SELECT` : Menunjukkan bahwa kita ingin mengambil semua kolom dari tabel "mobil".
`FROM mobil`: Menunjukkan bahwa pengambilan data dilakukan dari tabel "mobil".
`WHERE warna IN ('pink', 'biru') AND harga_rental = 50000`: Ini adalah klausa WHERE yang berfungsi sebagai filter untuk memilih baris yang memiliki nilai 'pink' atau 'biru' di kolom "warna" dan nilai 50000 di kolom "harga_rental".
## Kesimpulan
pernyataan SELECT ini akan mengambil semua kolom dari tabel "mobil" untuk data yang memiliki nilai "warna" sama dengan 'pink' atau 'biru' dan nilai "harga_rental" sama dengan 50000.
___
# IN/OR

## Struktur
```sql
select * from nama_tabel where data IN('nilai 1','nilai 2')OR data 2=nilai 1;
```
## Contoh Query
```sql
select * from mobil where warna IN('pink','biru')OR harga_rental=50000;
```
## Hasil
![gambarr](Aset/IMG_11.jpg)

## Analisis
`SELECT` : Pernyataan SELECT ini menunjukkan bahwa kita akan mengambil semua kolom dari tabel "mobil".

`FROM mobil`: Mengidentifikasi tabel yang akan digunakan dalam operasi SELECT, yaitu tabel "mobil".

`WHERE warna IN('pink','biru') OR harga_rental=50000`: Klausul WHERE digunakan untuk menerapkan kriteria seleksi pada data yang akan diambil. Dalam hal ini, data akan dipilih jika nilai kolom "warna" berada dalam daftar nilai yang diberikan ('pink' atau 'biru') atau nilai kolom "harga_rental" sama dengan 50000.
## Kesimpulan
pernyataan SELECT ini akan mengambil semua kolom dari tabel "mobil" untuk data yang memiliki nilai "warna" sama dengan 'pink' atau 'biru' atau nilai "harga_rental" sama dengan 50000.
# IN/AND/OPERATOR
## Struktur
```sql
select * from nama_tabel where data IN('nilai 1','nilai 2')AND data 2<nilai 1;
```
## Contoh Query
```sql
select * from mobil where warna IN('pink','biru')AND harga_rental<100000;
```
## Hasil
![gambar](Aset/IMG_12.jpg)

## Analisis
`SELECT` : Pernyataan SELECT ini menunjukkan bahwa kita akan mengambil semua kolom dari tabel "mobil".

`FROM mobil`: Mengidentifikasi tabel yang akan digunakan dalam operasi SELECT, yaitu tabel "mobil".

`WHERE warna IN('pink','biru') AND harga_rental<100000`: Klausul WHERE digunakan untuk menerapkan kriteria seleksi pada data yang akan diambil. Dalam hal ini, data akan dipilih jika nilai kolom "warna" berada dalam daftar nilai yang diberikan ('pink' atau 'biru') dan nilai kolom "harga_rental" kurang dari 100000.
## Kesimpulan
pernyataan SELECT ini akan mengambil semua kolom dari tabel "mobil" untuk data yang memiliki nilai "warna" sama dengan 'pink' atau 'biru' dan nilai "harga_rental" kurang dari 100000.
# LIKE (Mencari awalan)
## Struktur
```sql
select * from nama_tabel where data LIKE 'n%';
```
## Contoh Query
```sql
select * from mobil where pemilik LIKE 'J%';
```
## Hasil
![gambar](IMG_13.jpg)

## Analisis
`SELECT` : Pernyataan SELECT ini menunjukkan bahwa kita akan mengambil semua kolom dari tabel "mobil".

`FROM mobil`: Mengidentifikasi tabel yang akan digunakan dalam operasi SELECT, yaitu tabel "mobil".

`WHERE pemilik LIKE 'J%'`: Klausul WHERE digunakan untuk menerapkan kriteria seleksi pada data yang akan diambil. Dalam hal ini, data akan dipilih jika nilai kolom "pemilik" dimulai dengan huruf 'J' dan diikuti oleh nol atau lebih karakter tambahan.
## Kesimpulan
pernyataan SELECT ini akan mengambil semua kolom dari tabel "mobil" untuk data yang memiliki nilai kolom "pemilik" dimulai dengan huruf 'J'.
# LIKE (Mencari akhir)
## Struktur Query 
```sql
select * from nama_tabel where data LIKE '%n':
```
## Contoh Query
```sql
select * from mobil where pemilik LIKE '%n':
```
## Hasil
![gambar](Aset/IMG_14.jpg)

## Analisis
memilih semua baris dari tabel "mobil" di mana nilai kolom "pemilik" berakhir dengan huruf "n". Operator LIKE digunakan dengan pola pencocokan '%n', di mana '%' cocok dengan nol atau lebih karakter apa pun sebelum "n". Misalnya, jika ada entri dengan nilai kolom "pemilik" adalah "Jordan", entri itu akan dipilih karena akhirannya adalah "n"
## Kesimpulan
select * from mobil where pemilik LIKE '%n' digunakan untuk memilih semua baris dari tabel "mobil" di mana nilai kolom "pemilik" berakhir dengan huruf "n". Dengan menggunakan operator LIKE dan pola pencocokan %n
# LIKE (Mencari awalan/akhir)
## Struktur Query 
```sql
Select * from nama_tabel where data LIKE 'J%n';
```
## Contoh Query
```sql
Select * from mobil where pemilik LIKE 'J%n';
```
## Hasil
![gambar](Aset/IMG_15.jpg)

## Analisis
SELECT * FROM mobil WHERE pemilik LIKE 'J%n' digunakan untuk memilih semua baris dari tabel "mobil" di mana nilai kolom "pemilik" dimulai dengan huruf "J" dan berakhir dengan huruf apapun setelahnya. Dengan menggunakan operator LIKE dan pola pencocokan 'J%n'
## Kesimpulan
Program SQL SELECT * FROM mobil WHERE pemilik LIKE 'J%n' digunakan untuk memilih semua baris dari tabel "mobil" di mana nilai kolom "pemilik" dimulai dengan huruf "J", diikuti oleh nol atau lebih karakter, kemudian diikuti oleh satu karakter apa pun.
# LIKE(mencari total Karakter)
## Struktur Query 
```sql
Select * from nama_tabel where data LIKE 'n':
```
## Contoh Query
```sql
Select * from mobil where pemilik LIKE 'Jordan':
```
## Hasil

![gambar](Aset/IMG_16.jpg)

## Analisis
`SELECT * FROM mobil WHERE pemilik LIKE 'Jordan'` digunakan untuk memilih semua baris dari tabel "mobil" di mana nilai kolom "pemilik" sama dengan "Jordan". Dengan menggunakan operator LIKE dan pola pencocokan 'Jordan',
## Kesimpulan
Program SQL SELECT * FROM mobil WHERE pemilik LIKE 'Jordan' digunakan untuk memilih semua baris dari tabel "mobil" di mana nilai kolom "pemilik" adalah tepat "Jordan".
# LIKE(Kombinasi)
## Struktur Query 
```sql
Select * from nama_tabel where data LIKE '_%':
```
## Contoh Query
```sql
Select * from mobil where pemilik LIKE 'Jordan%':
```
## Hasil
![gambar](Aset/IMG_17.jpg)

## Analisis
SELECT * FROM mobil WHERE pemilik LIKE 'Jordan%' digunakan untuk memilih semua baris dari tabel "mobil" di mana nilai kolom "pemilik" dimulai dengan kata "Jordan". Dengan menggunakan operator LIKE dan pola pencocokan 'Jordan%', program ini mencari data di mana nilai kolom "pemilik" dimulai dengan kata "Jordan" diikuti oleh karakter apa pun atau tanpa karakter tambahan
## Kesimpulan
Program SQL SELECT * FROM mobil WHERE pemilik LIKE 'Jordan%' digunakan untuk memilih semua baris dari tabel "mobil" di mana nilai kolom "pemilik" dimulai dengan kata "Jordan", diikuti oleh nol atau lebih karakter tambahan.
# NOT LIKE
## Struktur Query 
```sql
Select * from nama_tabel where data NOT LIKE '_%':
```
## Contoh Query
```sql
Select * from mobil where pemilik NOT LIKE 'J%':
```
## Hasil

![gambar](Aset/IMG_18.jpg)

## Analisis
`SELECT * FROM mobil WHERE pemilik NOT LIKE 'J%'` digunakan untuk memilih semua baris dari tabel "mobil" di mana nilai kolom "pemilik" tidak dimulai dengan huruf "J". Dengan menggunakan operator NOT LIKE dan pola pencocokan 'J%'
## Kesimpulan
program ini mencari data di mana nilai kolom "pemilik" tidak dimulai dengan huruf "J".
# NULL 
## Struktur Query 
```sql
select * from nama_tabel where kolom_tabel IS NOT NULL;
```
## Contoh Query
```Sql
select * from mobil where peminjam IS NULL;
```
## Hasil 
![gambar](Aset/IMG_19.jpg)

## Kesimpulan
Program SQL tersebut merupakan perintah SELECT yang digunakan untuk mengambil semua data dari tabel "mobil" di mana nilai dalam kolom "pemilik" mengandung huruf "n" di mana pun posisinya.
# NOT NULL
## Struktur Query 
```sql
select * from nama_tabel where kolom_tabel IS NOT NULL;
```
## Contoh Query 
```sql
select * from mobil where peminjam IS NOT NULL;
```
## Hasil 
![gambar](Aset/IMG_20.jpg)

## Kesimpulan 
untuk mengambil semua data dari tabel "mobil" di mana kolom "peminjam" tidak kosong (tidak NULL).
# ORDER BY & LIMIT
## ORDER BY
### Struktur Query 
```sql
select * from nama_tabel ORDER BY kolom_tabel ASC;
```
### Contoh Query 
```sql
select * from mobil ORDER BY pemilik ASC;
```
## Hasil
![gambar](Aset/IMG_21.jpg)

## Kesimpulan
Perintah SQL tersebut digunakan untuk mengambil semua data dari tabel "mobil" dan mengurutkannya berdasarkan nilai pada kolom "pemilik" secara menaik (ASC).
## Struktur Query
```sql
select * from nama_tabel ORDER BY kolom_tabel ASC;
```
## Contoh Query 
``` sql
select * from mobil ORDER BY peminjam ASC;
```
## Hasil
![gambar](Aset/IMG_22.jpg)

## Kesimpulan 
Perintah SQL tersebut digunakan untuk mengambil semua data dari tabel "mobil" dan mengurutkannya berdasarkan nilai pada kolom "peminjam" secara menaik (ASC).
## LIMIT
### Contoh Query 
```Sql
SELECT * FROM mobil WHERE warna = ”Hitam” ORDER BY harga ASC LIMIT 2;
```

# DISTINCT
## Struktur Query 
```sql
select distinct (kolom_tabel) from nama_tabel;
```
## Contoh Query 
```sql
select distinct (pemilik) from mobil;
```
## Hasil
![gambar](Aset/IMG_23.jpg)

## Kesimpulan 
Perintah SQL tersebut digunakan untuk mengambil nilai unik dari kolom "pemilik" dalam tabel "mobil".

## Contoh Query 
```sql
select distinct (harga_rental) from mobil ORDER BY harga_rental desc;
```
## Hasil
![gambar](Aset/IMG_24.jpg)

## Kesimpulan 
Perintah SQL tersebut digunakan untuk mengambil nilai unik dari kolom "harga_rental" dalam tabel "mobil", kemudian hasilnya diurutkan secara menurun (descending) berdasarkan nilai harga_rental.
## CONCAT_WS

#### Contoh Query 
```sql
SELECT CONCAT_WS("-",no_plat,no_mesin,id_mobil) FROM mobil;
```
#### Hasil
![Gambar](Aset/IMG_25.jpg)

#### Analisis 
`SELECT`: Digunakan untuk memilih kolom yang akan ditampilkan dalam hasil query.

`CONCAT_WS("-", no_plat, no_mesin, id_mobil)`: Fungsi CONCAT_WS digunakan untuk menggabungkan nilai dari kolom "no_plat", "no_mesin", dan "id_mobil" dengan menggunakan pemisah "-" (dash) di antara setiap nilai. Hasil penggabungan tersebut akan menjadi satu nilai tunggal.

`FROM mobil`: Menunjukkan bahwa tabel yang digunakan dalam query ini adalah "mobil".

Hasil query ini menghasilkan satu kolom yang berisi nilai-nilai hasil penggabungan antara kolom "no_plat", "no_mesin", dan "id_mobil" dari setiap baris dalam tabel "mobil" dengan pemisah "-" di antara setiap nilai.
#### Kesimpulan 
Kesimpulannya Pada query ini, `SELECT CONCAT_WS("-", no_plat, no_mesin, id_mobil) FROM mobil;`, dilakukan seleksi data dari tabel "mobil" dengan menggabungkan  antara kolom "no_plat", "no_mesin", dan "id_mobil" menggunakan pemisah "-" (dash).

### AS

#### Contoh Query 
```sql
SELECT
CONCAT_WS("+",pemilik,peminjam) AS
COLLAB FROM mobil
```
#### Hasil

![gambar](Aset/IMG_26.jpg)

#### Analisis 
 `SELECT`: Digunakan untuk memilih kolom yang akan ditampilkan dalam hasil query.

`CONCAT_WS("+", pemilik, peminjam) AS COLLAB`: Fungsi CONCAT_WS digunakan untuk menggabungkan nilai dari kolom "pemilik" dan "peminjam" dengan menggunakan pemisah "+" (plus) di antara setiap nilai. Hasil penggabungan tersebut akan menjadi satu nilai . "COLLAB" diberikan pada kolom hasil penggabungan.

`FROM mobil`: Menunjukkan bahwa tabel yang digunakan dalam query ini adalah "mobil".

Hasil query tersebut akan menghasilkan satu kolom tunggal dengan nama "COLLAB" yang berisi nilai-nilai hasil penggabungan antara kolom "pemilik" dan "peminjam" dari setiap baris dalam tabel "mobil" dengan pemisah "+" di antara setiap nilai.
#### Kesimpulan 
Pada query SQL ini, `SELECT CONCAT_WS("+", pemilik, peminjam) AS COLLAB FROM mobil;`untuk menyeleksi data dari tabel "mobil" dengan melakukan penggabungan antara kolom "pemilik" dan "peminjam" menggunakan pemisah "+" (plus) sebagai CONCAT_WS. Hasil penggabungan diberi alias "COLLAB" pada hasil query.
## View
## Tantangan 
### 1. Buatkan tabel virtual dan tampilkan datanya yang mana peminjamannya itu tidak ada (NULL)

#### Contoh Query 
```sql
CREATE VIEW peminjam NULL AS SELECT id_mobil,no plat, peminjam, harga_rental FROM mobil WHERE peminjam IS NULL;
```

#### Hasil
![gambar](Aset/IMG_27.jpg)

### 2. update atau ganti salah satu data peminjam dari tabel mobil dengan nilai NULL, tampilkan isi data pada tabel 

#### Contoh Query 
```Sql
Update mobil SET peminjam=NULL WHERE id_mobil=3;
```

#### Hasil
#### before
![gambar](Aset/IMG_28.jpg)
#### after
![gambar](Aset/IMG_29.jpg)

### 3. Berikan Kesimpulan mengapa tabel virtual ini dibuat
Tabel virtual dalam MySQL dibuat untuk menyimpan hasil dari kueri SQL yang kompleks atau berulang, sehingga hasilnya dapat diakses dengan mudah dan efisien
## AGREGASI
### Sum
#### struktur query 
```sql
SELECT SUM(nama_kolom) AS total FROM nama_tabel
WHERE kondisi_opsional;
```
#### Contoh Query 
```sql
SELECT SUM(harga_rental) FROM mobil;
```

#### Hasil
![gambar](Aset/IMG_30.jpg)

#### Analisis 
`SELECT SUM(harga_rental)`: Ini adalah bagian dari pernyataan SELECT yang mengambil nilai total dari kolom "harga_rental". SUM digunakan untuk menjumlahkan nilai-nilai dalam kolom tertentu.

`FROM mobil`: Ini menunjukkan bahwa tabel yang digunakan dalam query ini adalah "mobil". Anda mengambil nilai dari kolom "harga_rental" di dalam tabel ini.
#### Kesimpulan 
Kesimpulannya,`SUM` ini akan menampilkan hasil penjumlahan dari seluruh penjumlahan `harga_rental` dari tabel mobil.

### Count
#### Struktur Query 
```
SELECT COUNT(*) AS jumlah FROM nama_tabel WHERE kondisi_opsional;
```
#### Contoh Query 
```sql
SELECT COUNT(pemilik) FROM mobil;
```

#### Hasil
![gambar](Aset/IMG_31.jpg)
#### Analisis 
`SELECT COUNT(pemilik)`: Perintah ini memilih kolom pemilik dari tabel mobil dan menghitung jumlah baris di mana nilai kolom pemilik tidak null.
`FROM mobil`: Ini menunjukkan bahwa kita sedang memilih data dari tabel bernama mobil.
#### Kesimpulan 
jumlah total baris dalam tabel mobil di mana kolom pemilik memiliki nilai yang tidak null. Misalnya, jika tabel mobil memiliki beberapa baris di mana pemilik diisi, perintah ini akan mengembalikan jumlah total baris tersebut.
#### Contoh Query 
```sql
SELECT COUNT(peminjam) FROM mobil;
```

#### Hasil
![gambar](IMG_32.jpg)
#### analisis 
`SELECT COUNT(peminjam)`: Perintah ini memilih kolom peminjam dari tabel mobil dan menghitung jumlah baris di mana nilai kolom peminjam tidak null.
`FROM mobil`: Ini menunjukkan bahwa kita sedang memilih data dari tabel bernama mobil.
#### Kesimpulan 
 jumlah total baris dalam tabel mobil di mana kolom peminjam memiliki nilai yang tidak null. Misalnya, jika tabel mobil memiliki beberapa baris di mana peminjam diisi, perintah ini akan mengembalikan jumlah total baris tersebut.


### Min
#### Struktur Query 
```sql
SELECT MIN(nama_kolom) AS nilai_minimum FROM nama_tabel

WHERE kondisi_opsional;
```
#### Contoh Query 
```sql
SELECT MIN(harga_rental) AS MINIMAL FROM mobil;
```

#### Hasil
![](Aset/IMG_33.jpg)

#### analisis 
- `SELECT COUNT(peminjam)`: Perintah ini memilih kolom `peminjam` dari tabel `mobil` dan menghitung jumlah baris di mana nilai kolom `peminjam` tidak null.
    
- `FROM mobil`: Ini menunjukkan bahwa kita sedang memilih data dari tabel bernama `mobil`.
#### Kesimpulan 
minimum dari kolom harga_rental dalam tabel mobil. Misalnya, jika terdapat beberapa nilai harga rental dalam tabel mobil, perintah ini akan mengembalikan nilai terkecil di antara mereka.
### Max
#### Struktur Query 
```sql
SELECT MAX(nama_kolom) AS nilai_maksimum FROM nama tabel
WHERE kondisi_opsional;
```
#### Contoh Query 
```sql
SELECT MAX(harga_rental) AS MAXIMAL FROM mobil;
```

#### Hasil
![gambar](Aset/IMG_34.jpg)
#### analisis 
- `SELECT MAX(harga_rental) AS MAXIMAL`: Perintah ini memilih nilai maksimum dari kolom harga_rental dalam tabel mobil dan memberikan alias MAXIMAL pada hasilnya.
- `FROM mobil`: Ini menunjukkan bahwa kita sedang memilih data dari tabel bernama mobil.
#### Kesimpulan 
 nilai maksimum dari kolom harga_rental dalam tabel mobil. Misalnya, jika terdapat beberapa nilai harga rental dalam tabel mobil, perintah ini akan mengembalikan nilai terbesar di antara mereka.
### AVG
#### Struktur Query 
```sql
SELECT AVG(nama_kolom) AS rata_rata FROM nama_tabel
WHERE kondisi_opsional;
```
#### Contoh Query 
```sql
SELECT AVG(harga_rental) AS RATA_RATA FROM mobil;
```

#### Hasil
![gamb](Aset/IMG_35.jpg)
#### analisis 
- `SELECT AVG(harga_rental) AS RATA_RATA`: Perintah ini menghitung nilai rata-rata dari kolom harga_rental dalam tabel mobil dan memberikan alias RATA_RATA pada hasilnya.
- `FROM mobil`: Ini menunjukkan bahwa kita sedang memilih data dari tabel bernama mobil.
#### Kesimpulan
nilai rata-rata dari kolom harga_rental dalam tabel mobil. Misalnya, jika terdapat beberapa nilai harga rental dalam tabel mobil, perintah ini akan mengembalikan rata-rata dari nilai-nilai tersebut.