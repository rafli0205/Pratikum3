## 1.Mencari Bilangan Terbesar dari 3 Variabel
Program sederhana menentukan bilangan terbesar daritiga angka yang diinputkan pengguna.
## Deskripsi Program
- Meminta user memasukan 3 bilanan berbeda
- Function tersebut menggunakan nested if-else statement untuk mebandingkan angka yang diinputkan
- Kemudian akan menampilkan mana bilangan terbesar
- Lalu kita panggil kembali function mencari_bilangan_terbesar
- Lalu Output bilangan terbesar dari ketiga bilangan yang di input akan muncul
## Flowchart Program
![Untitled Diagram](https://github.com/user-attachments/assets/f91727a0-8797-4b57-b1e9-6c0514954b5f)
## Kode Program
```Python
a = int(input("Masukkan bilangan A: "))
b = int(input("Masukkan bilangan B: "))
c = int(input("Masukkan bilangan C: "))

if a > b:
    if a > c:
        print("Terbesar adalah A")
        terbesar = a
    else:
        print("Terbesar adalah c")
        terbesar = c
else:
    if b > c:
        print("Terbesar adalah B")
        terbesar = b
    else:
        print("Terbesar adalah C")

print(f"Bilangan terbesar adalah: {terbesar}")
```
```Python
## Contoh Output
Masukkan bilangan A: 88
Masukkan bilangan B: 89
Masukkan bilangan C: 90
Terbesar adalah C
```
## Cara kerja
Menerima input 3 bilangan (A,B, C) dari user melakukan pengecekan dengan urutan: Apakah A > B? Jika ya: A adalah terbesar JIka tidak: C adalah terbesar Jika tidak: cek apakah B > C? Jika ya: B adalah terbesar Jika tidak: C adalah terbesar Menampilkan bilangan terbesar yang ditemukan.

## 2.Program Mencari Bilangan Terbesar
Program sederhana untuk mencari nilai terbesar dari sekumpulan bilangan yang di masukkan oleh pengguna menggunakan loop while True dan break statement.

## Deskripsi Program
Program di buat menggunakan bahasa python
- Menggunakan while True untuk perulangan tak terbatas
- Menggunakan break statement untuk menghentikan program
- Membandingkan setiap input dengan nilai maksimum yang tersimpan
- Menampilkan bilangan terbesar yang ditemukan

## Flowchart program
![Untitled Diagram (1)](https://github.com/user-attachments/assets/e58fcc23-13a0-46e9-88ea-5d38b2d696c9)
## Kode Program
```Python
max = 0                                              
while True:                                          
    bilangan = int(input("Masukan bilangan(0 untuk berhenti): "))  
    if bilangan == 0:                               
        break                                       
    if bilangan > max:                     
        max = bilangan                     
print(f"Bilangan terbesar: {max}")
```
```Python
## Contoh Output Program
Masukan bilangan(0 untuk berhenti): 78
Masukan bilangan(0 untuk berhenti): 89
Masukan bilangan(0 untuk berhenti): 57
Masukan bilangan(0 untuk berhenti): 38
Masukan bilangan(0 untuk berhenti): 78
Masukan bilangan(0 untuk berhenti): 0
Bilangan terbesar: 89
```
## Cara Kerja Program
Program berfungsi untuk mencari bilangan terbesar dari input yang diberikan pengguna. Pertama, prgram menginisialisasi variabel max dengan nilai o. Kemudian, program meminta pengguna untuk memasukkan bilangan. Jika bilangan yang dimasukkan bukan 0, program akan memeriksa apakah bilangan itu lebih besar dari nilai max. Jika iya, nilai max akan diperbarui dengan bilangan tersebut, Proses ini berulang hingga pengguna memasukkan 0, yang menandakan akhir dari input. Setelah itu, program mencetak bilangan terbesar yang ditemukan.

Namun, untuk meningkatkan program, bisa menginisialisasi max dengan None, sehingga dapat menangani situasi di mana pengguna langsung memasukkan 0 tanpa memberikan bilangan lain. Dengan cara ini, program akan lebih robust dan memberikan pesan yang sesuai jika tidak ada bilangan yang dimasukkan.
