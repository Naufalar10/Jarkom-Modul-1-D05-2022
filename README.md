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

## Soal 8

### Telusuri aliran paket dalam file .pcap yang diberikan, cari informasi berguna berupa percakapan antara dua mahasiswa terkait tindakan kecurangan pada kegiatan praktikum. Percakapan tersebut dilaporkan menggunakan protokol jaringan dengan tingkat keandalan yang tinggi dalam pertukaran datanya sehingga kalian perlu menerapkan filter dengan protokol yang tersebut.

a. Buka resource “soal8-10.pcapng”

b. Menulusuri packet, lalu menemukan paket pertama:
	
c. Dari packet ini, tarik kesimpulan bahwa kunci merupakan IP address 127.0.0.1 dan 127.0.1.1 dan TCP port 65432 dan 60236. Sehingga, filter yang dapat dipakai merupakan: (ip.src == 127.0.0.1 ||  ip.dst == 127.0.0.1) && (tcp.port == 65432 || tcp.port  == 60236). Dapat hasil berupa :

e. klik kanan salah satu paket tersebut. Lalu klik “Follow” dan klik “TCP stream”

f. Berikut ini transkrip percakapannya:


 ## Soal 9

### Terdapat laporan adanya pertukaran file yang dilakukan oleh kedua mahasiswa dalam percakapan yang diperoleh, carilah file yang dimaksud! Untuk memudahkan laporan kepada atasan, beri nama file yang ditemukan dengan format [nama_kelompok].des3 dan simpan output file dengan nama “flag.txt”.

a. Dari filter yang sama dengan soal no.8 tertemu percakapan sebagai berikut:

b. Oh oke2 deh, boleh sekalian kirimin file saltnya nggak? Hehe
Hilih yadeh, lewat 9002 ya?
c. Maka, dengan memakai filter (ip.src == 127.0.0.1 ||  ip.dst == 127.0.0.1) && +tcp.port == 9002 akan menemukan transmisi ini:

e. Jika kita menyalin data tersebut dalam bentuk raw lalu buka dengan command file dalam linux maka akan mendapat hasil sebagai berikut: 

f. Sehingga jika kita memasukkan passwordnya sesuai dengan no 10 (berupa nakano) kita dapat memasukkan command sebagai berikut:

g. Hasilnya akan sebagai berikut:

## Soal 10

### Temukan password rahasia (flag) dari organisasi bawah tanah yang disebutkan di atas!

a. dari filter yang sama dengan soal no. 8, tertemu percapakan sebagai berikut:
Ada, klo nggak salah passwordnya itu pake nama karakter anime yang kembar lima itu lho, jangan lupa pake huruf kecil semua
b. Dari percakapan tersebut, setelah mencoba-coba dengan file yang didapat pada soal no 9, dapat diketahui bahwa password yang dipakai adalah “nakano”
