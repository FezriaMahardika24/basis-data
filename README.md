# basis-data
<<<<<<< HEAD
 # 1. Buat sebuah database dengan nama latihan2!
mysql> create database latihan02;
=======
![gambar1](1/https://github.com/FezriaMahardika24/basis-data/blob/main/ss-output-basisdata/1.jpeg)

# 2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam database latihan1!

mysql>create table biodata (nama varchar (15), alamat varchar (15));
![gambar1](2/https://github.com/FezriaMahardika24/basis-data/blob/main/ss-output-basisdata/2.jpeg)

# 3. Tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom terakhir!
mysql> alter table biodata add column keterangan varchar (15);
mysql> desc biodata
![gambar1](3/https://github.com/FezriaMahardika24/basis-data/blob/main/ss-output-basisdata/3.jpeg)

# 4. Tambahkan kolom id (int 11) di awal (sebagai kolom pertama)!
 mysql> alter table biodata add column id int(11) first;
 ![gambar1](4/https://github.com/FezriaMahardika24/basis-data/blob/main/ss-output-basisdata/4.jpeg)

# 5. Sisipkan sebuah kolom dengan nama phone (varchar 15) setelah kolom alamat!
mysql> alter table biodata add column phone varchar(15) after alamat;
mysql> desc biodata;
![gambar1](5/https://github.com/FezriaMahardika24/basis-data/blob/main/ss-output-basisdata/5.jpeg)

# 6. Ubah tipe data kolom id menjadi char(11)!
mysql> alter table biodata modify column id char (11);
![gambar1](6/https://github.com/FezriaMahardika24/basis-data/blob/main/ss-output-basisdata/6.jpeg)

# 7. Ubah nama kolom phone menjadi hp (varchar 20)!
mysql> alter table biodata change column phone hp varchar(20);
mysql> desc biodata;
![gambar1](7/https://github.com/FezriaMahardika24/basis-data/blob/main/ss-output-basisdata/7.jpeg)

# 8. Tambahkan kolom email setelah kolom hp!
mysql> alter table biodata add column email varchar(11) after hp;
mysql> desc biodata;
![gambar1](8/https://github.com/FezriaMahardika24/basis-data/blob/main/ss-output-basisdata/8.jpeg)

# 9. Hapus kolom keterangan dari tabel!
mysql> alter table biodata drop column keterangan;
![gambar1](9/https://github.com/FezriaMahardika24/basis-data/blob/main/ss-output-basisdata/9.jpeg)

# 10. Ganti nama tabel menjadi data_mahasiswa!
mysql> alter table biodata rename data_mahasiswa;
mysql> desc data_mahasiswa;
![gambar1](10/https://github.com/FezriaMahardika24/basis-data/blob/main/ss-output-basisdata/10.jpeg)

# 11. Ganti nama field id menjadi nim!
mysql> alter table data_mahasiswa change id nim;
mysql> desc data_mahasiswa;
![gambar1](11/https://github.com/FezriaMahardika24/basis-data/blob/main/ss-output-basisdata/11.jpeg)

# 12. Jadikan nim sebagai PRIMARY KEY!
mysql>  alter table data_mahasiswa add primary key (nim);
mysql> desc data_mahasiswa;
![gambar1](12/https://github.com/FezriaMahardika24/basis-data/blob/main/ss-output-basisdata/12.jpeg)

# 13. Jadikan kolom email sebagai UNIQUE KEY
mysql> alter table data_mahasiswa add unique key (email);
mysql> desc data_mahasiswa;
![gambar1](13/https://github.com/FezriaMahardika24/basis-data/blob/main/ss-output-basisdata/13.jpeg)

# C.	Data dan Analisis 
## 1.	Apa maksud dari Int (11)?
Maksud dari int (11) adalah nama tipe datanya adalah integer dan memiliki panjang 11 karakter.
## 2.	Ketika kita melihat sturktur tabel dengan perintah desc, ada kolom Null yang berisi Yes dan No, apa maksudnya?
Null di Mysql adalah istilah atau tipe data khusus dalam pemograman yang menyatakan ‘tidak ada nilai’, NULL tidak sama dengan 0, atau ‘’(string kosong). Apabila Null berisi no, maka data tersebut nantinya akan dilakukan pengisian atau penginputan. Sedangkan apabila Null berisi yes, maka artinya data tersebut akan dikosongkan atau tidak dilakukan penginputan.










=======



>>>>>>> 026813af7fa049f74b5ee14a7526eaf48edf779c