# Lapres Jarkom Modul 1 Kelompok D05 #

| Nama Praktikan  | NRP Praktikan |
| ------------- | ------------- |
| Ichlasul Hasanat  | 5025201091  |
| Haidar Fico Ramadhan Aryputra | 5025201185  |
| Naufal Ariq Putra Yosyam | 5025201112 |

## Soal 1 

### Sebutkan web server yang digunakan pada "monta.if.its.ac.id"!

### Jawab :
a. Masukkan wireshark filter expression “http.host == monta.if.its.ac.id” :
![1.1](https://github.com/Naufalar10/Jarkom-Modul-1-D05-2022/blob/main/image/gambar1.1.png)
b. Lalu klik kanan, klik follow, dan klik tcp stream :
![1.2](https://github.com/Naufalar10/Jarkom-Modul-1-D05-2022/blob/main/image/gambar1.2.png)
c. Lalu hasilnya akan kelihatan yaitu webserver nginx/1.10.3 :
![1.3](https://github.com/Naufalar10/Jarkom-Modul-1-D05-2022/blob/main/image/gambar1.3.png)

## Soal 2

### Ishaq sedang bingung mencari topik ta untuk semester ini , lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id” , judul TA apa yang dibuka oleh ishaq ?

### Jawab :
a. Masukkan wireshark filter expression “http.host == monta.if.its.ac.id” :
![2.1](https://github.com/Naufalar10/Jarkom-Modul-1-D05-2022/blob/main/image/gambar2.1.png)
b. lalu klik paket no.576 sehingga muncul info tentang paket 576
c. lalu copy alamat http://monta.if.its.ac.id/index.php/topik/detailTopik/194
d. lalu buka alamat link tersebut di browser :
![2.2](https://github.com/Naufalar10/Jarkom-Modul-1-D05-2022/blob/main/image/gambar2.2.png)
e. Maka judul TA yang dibuka Ishaq adalah “Evaluasi unjuk kerja User Space
FileSystem(FUSE)”

## Soal 3

### Filter sehingga wireshark hanya menampilkan paket yang menuju port 80!

### Jawab :
a. Buka file resource “soal3-6.pcapng”
b. Masukkan wireshark filter expression “tcp.dstport == 80” ke dalam display filter
c. Berikut tampilannya:
![3](https://github.com/Naufalar10/Jarkom-Modul-1-D05-2022/blob/main/image/gambar3.png)

## Soal 4

### Filter sehingga wireshark hanya mengambil paket yang berasal dari port 21!

### Jawab :
a. Buka resource “Soal 3-6”
b. Masukkan wireshark filter expression “tcp.srcport ==21” ke dalam display filter
c. Berikut tampilannya:
![4](https://github.com/Naufalar10/Jarkom-Modul-1-D05-2022/blob/main/image/gambar4.png)

## Soal 5

### Filter sehingga wireshark hanya mengambil paket yang berasal dari port 443!

### Jawab :
a. Buka file resource “soal3-6.pcapng”
b. Masukkan “tcp.srcport == 443” ke dalam display filter
Berikut tampilannya:

![5](https://github.com/Naufalar10/Jarkom-Modul-1-D05-2022/blob/main/image/gambar5.png)

## Soal 6

### Filter sehingga wireshark hanya menampilkan paket yang menuju ke lipi.go.id!

### Jawab :
a. Buka resource “Soal 3-6”
b. Masukkan “ip.dst == lipi.go.id” ke dalam display filter
Berikut tampilannya:

![6](https://github.com/Naufalar10/Jarkom-Modul-1-D05-2022/blob/main/image/gambar6.png)

## Soal 7

### Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!

### Jawab :
a. Buka command prompt
b. Input “ipconfig” untuk melihat IPv4
Berikut contoh outputnya:

![7.1](https://github.com/Naufalar10/Jarkom-Modul-1-D05-2022/blob/main/image/gambar7.1.png)

c. Buka wireshark dan buka wifi

![7.2](https://github.com/Naufalar10/Jarkom-Modul-1-D05-2022/blob/main/image/gambar7.2.png)

d. Masukkan “ip.src_host == [ip address]”. Disini saya masukkan ip address = 192.168.0.104
Berikut outputnya:

![7.3](https://github.com/Naufalar10/Jarkom-Modul-1-D05-2022/blob/main/image/gambar7.3.png)

