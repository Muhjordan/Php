

# TABEL Employees

>![Foto_hasil](aset/IMG-2.jpg)




# TABEL Orders

>![Foto_hasil](aset/IMG-4.jpg)



---





# 1


## Query 

```MySQL



```


## Hasil



## Analisis 






---



# 2
## Query

```sql
SELECT * FROM employees;
```
## Hasil
![gambar](tabel.png)
## Analisis
- **SELECT**: Ini adalah kata kunci dalam SQL yang digunakan untuk memilih atau mengambil data dari database.
    
- ***** (Asterisk): Tanda asterisk digunakan sebagai wildcard yang berarti "semua kolom". Jadi, perintah ini akan mengambil semua kolom yang tersedia di tabel yang ditentukan.
    
- **FROM employees**: Ini adalah klausa FROM yang menunjukkan tabel yang akan digunakan untuk mengambil data. Dalam hal ini, tabel yang digunakan adalah "employees".

# 3
## Query
```sql
SELECT EmpID,Lastname,City FROM Employees;
```
## Hasil
![gambar](2.png)
## Analisis
- **SELECT**: Ini adalah kata kunci dalam SQL yang digunakan untuk memilih atau mengambil data dari database.
    
- **EmpID, Lastname, City**: Ini adalah nama kolom yang ingin Anda ambil dari tabel "Employees".
    
- **FROM Employees**: Ini adalah klausa FROM yang menunjukkan tabel yang akan digunakan untuk mengambil data. Dalam hal ini, tabel yang digunakan adalah "Employees".
# 4
## Query
```sql
Select empID, LaseName, City From Employees WHERE City = "Seattle"
```
## Hasil
![nama](no4b.png)
## Analisis
- **SELECT**: Ini adalah kata kunci dalam SQL yang digunakan untuk memilih atau mengambil data dari database.
    
- **EmpID, LastName, City**: Ini adalah nama kolom yang ingin Anda ambil dari tabel "Employees".
    
- **FROM Employees**: Ini adalah klausa FROM yang menunjukkan tabel yang akan digunakan untuk mengambil data. Dalam hal ini, tabel yang digunakan adalah "Employees".
    
- **WHERE City = 'Seattle'**: Ini adalah klausa WHERE yang memberikan kriteria untuk mengambil data. Dalam hal ini, kita hanya akan mengambil data di mana nilai kolom "City" sama dengan "Seattle".


## Query 

```MySQL



```


## Hasil



## Analisis 






---




# 5


## Query 

```MySQL



```


## Hasil



## Analisis 







---




# 6


## Query 

```MySQL



```


## Hasil



## Analisis 






---




# 7


## Query 

```MySQL



```


## Hasil



## Analisis 







---




# 8


## Query 

```MySQL



```


## Hasil



## Analisis 







---




# 9


## Query 

```MySQL



```


## Hasil



## Analisis 






---



# 10


## Query 

```MySQL



```


## Hasil



## Analisis 







----


# 11

## Query

```mysql
INSERT INTO tabel_guru (OrderID, CustID, EmpID, OrderDate, RequiredDate, ShippedDate, ShipVia)
    -> VALUES
    -> (10256, 'EASTC', 3, '1994-08-15', '1994-09-12', '1994-08-17', 2),
    -> (10257, 'SEVES', 4, '1994-08-16', '1994-09-13', '1994-08-22', 3),
    -> (10258, 'MAISD', 1, '1994-08-16', '1994-09-14', '1994-08-23', 1),
    -> (10259, 'ALFKI', 4, '1994-08-18', '1994-09-15', '1994-08-25', 3),
    -> (10260, 'ISLAT', 4, '1994-08-19', '1994-09-16', '1994-08-29', 1);
```


## Hasil

>![Foto_hasil](aset/IMG-5.jpg)



## Analisis

Program ini adalah contoh output dari sebuah tabel "orders" dalam format yang mirip dengan tabel yang ada dalam database relasional. Tabel ini mungkin digunakan untuk melacak pesanan dalam sebuah sistem, dan setiap baris mewakili satu pesanan dengan informasi yang terkait.
1. **OrderID**: Ini adalah ID unik untuk setiap pesanan. Setiap pesanan memiliki nomor ID yang berbeda.
2. **CustID**: Ini adalah ID atau kode pelanggan yang melakukan pesanan. Setiap pelanggan memiliki kode yang berbeda. Perhatikan bahwa untuk OrderID 10260, nilai CustID diganti dari 'ALFKI' menjadi 'ISLAT'.
3. **EmpID**: Ini adalah ID karyawan yang memproses pesanan.
4. **OrderDate**: Ini adalah tanggal ketika pesanan dibuat.
5. **RequiredDate**: Ini adalah tanggal ketika pelanggan meminta pesanan tersebut harus dipenuhi.
6. **ShipVia**: Ini mungkin adalah metode pengiriman yang digunakan untuk pesanan tersebut.
7. **ShippedDate**: Ini adalah tanggal ketika pesanan dikirim.

- Memeriksa bagaimana data ini digunakan dalam sistem yang lebih besar.
- Melakukan analisis tren pada data pesanan dari waktu ke waktu.
- Melakukan pemrosesan lebih lanjut atau analisis statistik terhadap pesanan, misalnya, total penjualan, rata-rata jumlah pesanan, atau metode pengiriman yang paling umum digunakan.



---


# 12

## Query

```mysql
select * from orders where empid = 1;
```



## Hasil

>![Foto_hasil](aset/IMG-6.jpg)



## Analisis

Output program menunjukkan satu baris data dari tabel orders. Berikut adalah analisis singkat

1. **OrderID**: Nomor pesanan adalah 10258.
2. **CustID**: Kode pelanggan yang melakukan pesanan adalah 'MAISD'.
3. **EmpID**: Karyawan dengan ID 1 yang memproses pesanan.
4. **OrderDate**: Pesanan dibuat pada tanggal 16 Agustus 1994.
5. **RequiredDate**: Pelanggan meminta pesanan harus dipenuhi pada tanggal 14 September 1994.
6. **ShipVia**: Metode pengiriman yang digunakan adalah 1.
7. **ShippedDate**: Pesanan dikirim pada tanggal 23 Agustus 1994.

Analisis program ini terbatas pada satu baris data, sehingga informasi yang diberikan tidak memberikan gambaran yang lengkap tentang kinerja keseluruhan sistem atau tren pesanan. Namun, kita dapat menyimpulkan bahwa pesanan ini diproses dengan sukses, dan pengiriman dilakukan dalam waktu yang wajar, yaitu pada tanggal 23 Agustus 1994, beberapa hari setelah pesanan dibuat.



---



# 13

## Query

```mysql
SELECT OrderID From orders where EmpID = 1;
```



## Hasil

>![Foto_hasil](aset/IMG-7.jpg)



## Analisis

Query ini bertujuan untuk menampilkan OrderID dari pesanan yang diproses oleh karyawan dengan ID 1. Output dari query ini adalah OrderID dari pesanan-pesanan tersebut. Dalam hal ini, hanya satu pesanan yang diproses oleh karyawan dengan ID 1, yaitu pesanan dengan OrderID 10258.




---





# 14


## QUERY

```MySQL

SELECT MIN(EmpyID) FROM Employees WHERE City = "Seattle";

```


## HASIL

>![Foto_hasil](aset/IMG-1.jpg)


## ANALISIS

1. **Fungsi Agregasi: `MIN`**
    
    - Fungsi `MIN` digunakan untuk mencari nilai minimum dari kolom yang ditentukan. Dalam hal ini, kolom yang ditentukan adalah `EmpyID`.
2. **Kolom yang Dipilih: `EmpyID`**
    
    - Kode tersebut memilih kolom `EmpyID` dari tabel `Employees`.
3. **Kondisi `WHERE`:**
    
    - Kondisi `WHERE` membatasi hasil query hanya pada baris-baris di mana nilai kolom `City` adalah "Seattle".
4. **Tabel yang Ditargetkan: `Employees`**
    
    - Query ini dijalankan pada tabel `Employees`.

Secara keseluruhan, query ini mencari nilai `EmpyID` terkecil di antara semua baris dalam tabel `Employees` yang memiliki `City` bernilai "Seattle".





---



# 15


## Query 

```MySQL

SELECT OrderID FROM Orders WHERE EmpID = (SELECT MIN(EmpyID) FROM Employees WHERE City = "Seattle");

```


## Hasil 

>![Foto_hasil](aset/IMG-3.jpg)



## Analisis 


1. **Tujuan:** Mendapatkan `OrderID` dari tabel `Orders` yang ditempatkan oleh karyawan dengan `EmpyID` terkecil di kota Seattle.
    
2. **Subquery:**
    
    - Menemukan `EmpyID` terkecil dari karyawan di Seattle:
        
3. **Query Utama:**
    
    - Memilih `OrderID` dari tabel `Orders` di mana `EmpID` sama dengan hasil dari subquery tersebut.


 Pastikan `EmpyID` adalah nama kolom yang benar.
 Indeks pada kolom `City` (tabel `Employees`) dan `EmpID` (tabel `Orders`) dapat meningkatkan kinerja.




