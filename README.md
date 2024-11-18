
# NAMA : MUHAMMAD GALIH FERI ABDILLLAH 
# NIM  : 312410299
# KELAS: TI.24.A4
# MATKUL : BAHASA PEMOGRAMAN
# LATIHAN PRAKTIKUM 5
![2](https://github.com/user-attachments/assets/4801c198-9ddc-43ba-91bb-0efff6236417)

# ELEMEN PY 
```python

list_a = [1, 2, 3, 4, 5]

print(list_a[2])

print(list_a[1:4])

print(list_a[-1])

list_a[3] = 10
print(list_a)

list_a[3:] = [11, 12, 13]
print(list_a)

list_b = list_a[:2]
print(list_b)

list_b.append("misalnya")
print(list_b)

list_b.extend([14, 15, 16])
print(list_b)

list_a.extend(list_b)
print(list_a) 
```
# CODE PROGRAM DI VISUAL CODE SEPERTI BERIKUT :
![PY 1](https://github.com/user-attachments/assets/f8c082e1-04ff-4064-87f0-0b55f49d4a5e)

# HASIL DARI CODINGAN YANG ADA DI ATAS SEBAGAI BERIKUT :
![PY 1](https://github.com/user-attachments/assets/97db030c-9806-4d0e-9b2e-6e367aaeaa85)

# MENAMBAH DATA PY :
 ```python
class Mahasiswa:
    def _init_(self, nama, nim, nilai_tugas, nilai_uts, nilai_uas):
        self.nama = nama
        self.nim = nim
        self.nilai_tugas = nilai_tugas
        self.nilai_uts = nilai_uts
        self.nilai_uas = nilai_uas

    def hitung_nilai_akhir(self):
        return (self.nilai_tugas + self.nilai_uts + self.nilai_uas) / 3

mahasiswa = []

while True:
    nama = input("Nama: ")
    nim = int(input("NIM: "))
    nilai_tugas = int(input("Nilai Tugas: "))
    nilai_uts = int(input("Nilai UTS: "))
    nilai_uas = int(input("Nilai UAS: "))

    mahasiswa.append(Mahasiswa(nama, nim, nilai_tugas, nilai_uts, nilai_uas))

    tambah_data = input("Tambah data (y/t)? ")
    if tambah_data.lower() == "t":
        break

print("-" * 60)
print("| No | Nama       | NIM  | Tugas | UTS  | UAS  | Akhir     |")
print("-" * 60)

for i, mhs in enumerate(mahasiswa):
    nilai_akhir = mhs.hitung_nilai_akhir()
    print(f"| {i+1:<2} | {mhs.nama:<10} | {mhs.nim:<4} | {mhs.nilai_tugas:<5} | {mhs.nilai_uts:<5} | {mhs.nilai_uas:<5} | {nilai_akhir:<9.2f} |")

print("-" * 60)
```
# PENJELASAN DARI CODE MENAMBAH DATA :
```python
class Mahasiswa:
    def __init__(self, nama, nim, nilai_tugas, nilai_uts, nilai_uas):
        self.nama = nama
        self.nim = nim
        self.nilai_tugas = nilai_tugas
        self.nilai_uts = nilai_uts
        self.nilai_uas = nilai_uas
__init__: Konstruktor ini digunakan untuk menginisialisasi objek Mahasiswa dengan atribut: nama, nim, nilai_tugas, nilai_uts, nilai_uas

def hitung_nilai_akhir(self):
    return (self.nilai_tugas + self.nilai_uts + self.nilai_uas) / 3
```
# METODE INI MENGEMBALIKAN NILAI AKHIR MAHASISWA YANG MERUPAKAN RATA-RATA DARI NILAI_TUGAS,NILAI_UTS,NILAI_UAS
```python
mahasiswa = []
```
# sebuah daftar kosong mahasiswa disiapkan untuk meyimpan objek mahasiswa yang akan di tambahkan 
```python
while True:
    nama = input("Nama: ")
    nim = int(input("NIM: "))
    nilai_tugas = int(input("Nilai Tugas: "))
    nilai_uts = int(input("Nilai UTS: "))
    nilai_uas = int(input("Nilai UAS: "))

    mahasiswa.append(Mahasiswa(nama, nim, nilai_tugas, nilai_uts, nilai_uas))

    tambah_data = input("Tambah data (y/t)? ")
    if tambah_data.lower() == "t":
        break
```
# meminta pengguna untuk memasukkan data mahasiswa berulang kali hingga pengguna memasukkan T untuk berhenti, setiap input digunakan untuk membuat data mahasiswa,yang kemudian ditambah kedalam daftar mahasiswa
```python
print("-" * 60)
print("| No | Nama       | NIM  | Tugas | UTS  | UAS  | Akhir     |")
print("-" * 60)

for i, mhs in enumerate(mahasiswa):
    nilai_akhir = mhs.hitung_nilai_akhir()
    print(f"| {i+1:<2} | {mhs.nama:<10} | {mhs.nim:<4} | {mhs.nilai_tugas:<5} | {mhs.nilai_uts:<5} | {mhs.nilai_uas:<5} | {nilai_akhir:<9.2f} |")

print("-" * 60)
```
# Header tabel dicetak terlebih dahulu, diikuti oleh baris-baris data untuk setiap mahasiswa, Untuk setiap mahasiswa, metode hitung_nilai_akhir dipanggil untuk menghitung nilai akhir, lalu data ditampilkan dalam format tabel

# CODE PROGRAM DI VISUAL CODE SEBAGAI BERIKUT : 
![PY2](https://github.com/user-attachments/assets/26401f3c-2b47-427f-90b8-bfd7766ad602)

# HASIL PROGRAM YANG ADA DI ATAS SEBAGAI BERIKUT :
![py 2](https://github.com/user-attachments/assets/e306f781-255a-4ff4-ba83-ed1774d46818)

# DAN DI BAWAH INI ADALAH FLOWCHARTNYA : 
![image](https://github.com/user-attachments/assets/b3a42627-efd3-4efa-81b4-825edce94563)








