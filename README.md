# Pertemuan_13-Exception

- Nama : Doni Perdana Siringoringo
- NIM  : 312210687
- Kelas: TI.22.B1

# Contoh dan Penjelasan Modul Praktikum 13

# 1. Berikut adalah fungsi yang mengubah suhu dari derajat derajat Kelvin menjadi derajat Fahrenheit. Karena nol derajat derajat Kelvin sedingin yang didapat, fungsi tersebut ditebus jika melihat suhu negatif.

![image](https://user-images.githubusercontent.com/115882455/208314455-dcac88f4-030b-47fe-98e0-8487b31eb05b.png)

# Ketika kode di atas dijalankan, muncul Exception yang bernama Traceback... AssertionError artinya terjadi error pada pernyataan assert.

# 2. Contoh ini untuk membuka file, menulis konten di file dan keluar dengan lancar karena tidak ada masalah sama sekali.

![image](https://user-images.githubusercontent.com/115882455/208314536-24c52626-e302-4ea2-b937-0d73d242f667.png)

# Hasilnya :
```
Written content in the file successfully
```
Hasilnya seperti ini karena else akan dijalankan ketika try adalah True

# 3. Contoh ini mencoba membuka file di mana Anda tidak memiliki izin menulis, sehingga menimbulkan pengecualian.

![image](https://user-images.githubusercontent.com/115882455/208314667-c4192bec-bb2a-4352-b410-310a1ac8ea62.png)

# Mengapa hasilnya error?
r adalah read - Membuka file untuk membaca, akan error jika file tidak ada. Disini ingin membaca file bukan menulis maka dibawahnya `fh = open("testfile", "r")` tambahkan `print(fh.readline())` dan fh.write dihapus. Setelah dijalankan, try dan else ditampilkan.

# 4. Contoh keempat

![image](https://user-images.githubusercontent.com/115882455/208314767-84e1d9be-6512-4989-b335-f691ef307e7f.png)

# Hasil diatas bukan error, karena finally dijalankan ketika try dan except dijalankan. Dan berhasil dibuat filenya setelah dijalankan.

# 5. Contoh single exception

![image](https://user-images.githubusercontent.com/115882455/208314801-ecbb69e2-e4a8-49e5-bf2e-4e7eac1602c5.png)

# Hasilnya :
```
The argument does not contain numbers 
invalid literal for int() with base 10: 'xyz'
```
# ketika dijalankan, maka muncul error. Hapus #!/usr/bin/python dan di except ValueError, Argument: ganti koma dengan as seperti except ValueError as Argument:agar tidak error. Jika dijalankan akan muncul error lagi. Kenapa? karena parameter def temp_convert harus mengandung angka.

# 6. Contoh dan penjelasan keenam

![image](https://user-images.githubusercontent.com/115882455/208314866-b06ff5b9-728f-4e9a-8b12-76b7903e985b.png)

# jika dijalankan muncul SyntaxError artinya ada kesalahan sintaks. Pada raise `"Invalid level!", level` ganti tanda koma dengan tanda plus. Cetak def dengan angka yang lebih besar dari 1.

# Selesai

#semogah bermanfaat


