# Program Data Mahasiswa

## Tampilan Syntax:

![python code](https://user-images.githubusercontent.com/56240498/69288713-ec410580-0c2c-11ea-97b0-7ff51947bf79.png)

## Algoritmanya:
1. Pertama kita membuat variable List dan juga Variable True:untuk perulanganya
```python
nilai = []
ulang = True
```
2.Buatlah Kondisi Perulangan yang sekarang.

![python code - Copy (2)](https://user-images.githubusercontent.com/56240498/69288640-bdc32a80-0c2c-11ea-956f-ef5ad35e5ea0.png)


- Hasil syntax di atas bertuliskan,Input nama, nim, nilai tugas, nilai uts, dan nilai uas, Dan System akan menjumlahkan nilai-nilai Secara otomatis dan menghasilkan nilai akhir dengan dibagikan dari setiap hasil tugas,uts,dan uas. Setelah menginput, inputan tersebut akan masuk ke dalam list 'nilai'.

3. Lalu kita akan membuat statement dimana program akan berhenti jika kita menlis kata 'T'.
```python
    if (input("Tambah data (y/t)?") == 't'):
        ulang = False
```

4. Terakhir adalah menyamakan sebuah tabel pada program yang akan di cetak,dengan menggunakan d,s,f dan juga mengurutkan variable dengan menggunakan format dan disambung dengan item agar mereka berurutan sehingga menjadi tabel yg sempurna.
```python
print("\n                      Daftar Nilai Mahasiswa")
print("==================================================================")
print("|No. |     Nama     |    NIM    | Tugas |  UTS  |  UAS  |  Akhir |")
print("==================================================================")
i = 0
for item in nilai:
    i += 1
    print("| {no:2d} | {nama:12s} | {nim:9s} | {tugas:5d} | {uts:5d} | {uas:5d} | {akhir:6.2f} |"
          .format(no=i, nama=item[0], nim=item[1], tugas=item[2], uts=item[3], uas=item[4], akhir=item[5]))
print("==================================================================")
``` 
