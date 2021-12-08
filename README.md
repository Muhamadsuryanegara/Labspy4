# Labspy4

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
    <table border="1">
        <tr>
            <th> Nama</th>
            <th>NIM</th>
            <th>Kelas</th>
        </tr>
        <tr>
            <td>Muhamad Suryanegara</td>
            <td>312110447</td>
            <td>TI.21.A.1</td>
        </tr>
    </table>
</body>
</html>

# List Python

## Tugas Latihan
![soal](https://user-images.githubusercontent.com/92678339/145260717-6c81b6cf-712f-4a53-b737-da05b2ac1275.png)

- Buat sebuah list sebanyak 5 elemen dengan nilai bebas
```bash
a = [10, 11, 13, 16, 17]
```
### Akses list:
- tampilkan elemen ke 3
```bash
print(a[2])
```
output !![Gambar 01](https://user-images.githubusercontent.com/92678339/145260856-42eb6270-b088-48b6-83c3-9f3b035770aa.png)<P>
- ambil nilai elemen ke 2 sampai elemen ke 4
```bash
print(a[1:4])
```
output ![hasil2](https://user-images.githubusercontent.com/92678339/145260896-45d00171-f3f9-4202-9fbc-7d64ff82dc22.png)<p>
- ambil elemen terakhir
```bash
print(a[-1])
```
output ![hasil3](https://user-images.githubusercontent.com/92678339/145261053-c10347a8-26d7-4f85-bd91-c40ddf63b70c.png)<p>
### Ubah elemen list:
- ubah elemen ke 4 dengan nilai lainnya
```bash
a[3] = 20
print(a)
```
output ![hasil4](https://user-images.githubusercontent.com/92678339/145260946-08fbd27d-5a89-4e22-80b6-68198dcf127e.png)<p>
- ubah elemen ke 4 sampai dengan elemen terakhir
```bash
a[3:] = [30, 22]
print(a)
```
output ![hasil5](https://user-images.githubusercontent.com/92678339/145261000-e4347ada-e9b0-43bc-9875-85e732712ed2.png)<p>
### tambah elemen list:
- ambil 2 bagian dari list pertama (A) dan jadikan list ke 2 (B)
```bash
b = a[0:2]
print (b)
```
output ![hasil6](https://user-images.githubusercontent.com/92678339/145261100-9da0f58d-979b-45c5-9bd6-c10a2a774af4.png)<p>
- tambah list B dengan nilai string
```bash
b.append('belajar')
print(b)
```
output ![hasil7](https://user-images.githubusercontent.com/92678339/145261132-b33669da-e877-4028-8c17-cd364519834e.png)<p>
- tambah list B dengan 3 nilai
```bash
b.extend([100, 30, 21])
print(b)
```
output ![hasil8](https://user-images.githubusercontent.com/92678339/145261165-7d960a6c-6355-4ba0-97c5-644ce4667615.png)<p>
- gabungkan list B dengan list A
```bash
b.extend(a)
print(b)
```
output ![Gambar 09](https://user-images.githubusercontent.com/92678339/145261208-4af83920-3172-447d-a4c8-f4959ec46118.png)<p>

### full my program
! [](https://user-images.githubusercontent.com/92678339/145261538-2062bcb0-2d24-4077-a7b2-499d283a3e50.png)<p>
- Output<p>
![Screenshot (88)](https://user-images.githubusercontent.com/92678339/145261705-84ad9bf9-5f03-47e1-99ce-bf29b75c9073.png)<p>


## Tugas Pratikum
- Soal<p>
![tugas pratikum](https://user-images.githubusercontent.com/92678339/145261761-989f5bd4-45a7-4334-b227-aa60413f7d02.png)
## Program
```bash
#program table data dengan perulangan
nama_list = []
nim_list = []
tugas_list = []
uts_list = []
uas_list = []
rata = []
a = 0
while True:
    nama_list.append(str(input("Nama\t\t : ")))
    nim_list.append(int(input("NIM\t\t : ")))
    tugas = int(input("Nilai Tugas\t : "))
    uts = int(input("Nilai UTS\t : "))
    uas = int(input("Nilai UAS\t : "))
    tugas_list.append(tugas)
    uts_list.append(uts)
    uas_list.append(uas)
    rata.append(tugas * .3 + uts * .35 + uas * .35)
    menambah = input("Ingin menambah data lagi? (Y/T):  ")
    if menambah =="t" or menambah =="T" :
        break
print()
print (68*"=")
print("| {0:^3} | {1:^12} | {2:^9} | {3:^6} | {4:^5} | {5:^5} | {6:^5} |".format("NO", "Nama", "NIM", "Tugas", "UTS", "UAS", "Akhir"))
print (68*"=")
no = 0
for nama, nim, tugas, uts, uas, akhir in zip (nama_list, nim_list, tugas_list, uts_list, uas_list, rata):
    no += 1
    print("| {0:^3} | {1:<12} | {2:>9} | {3:>6} | {4:>5} | {5:>5} | {6:>5} |".format(no, nama, nim, tugas, uts, uas, akhir))
print (68*"=")
```
- <b>Hasil Program</b><p>
![Screenshot (89)](https://user-images.githubusercontent.com/92678339/145262149-f033f284-00a6-4a69-b47f-fe70a94b0992.png)<p>
- <b>Penjelasan tentang program</b><p>
Program di atas adalah program list penginputan data dengan Looping/perulangan<p>
untuk perulangan nya sendiri saya juga menggunakan zip, karena saya butuh lebih dari satu iterable maka saya menambahkan zip di program ini<p>
Fungsi zip() mengembalikan nilai sesuai dengan argumen yang diberikan.<P>
<p>
# END
