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
(gambar)
b. Lalu klik kanan, klik follow, dan klik tcp stream :
(gambar)
c. Lalu hasilnya akan kelihatan yaitu webserver nginx/1.10.3 :
(gambar)

## Soal 2

### Ishaq sedang bingung mencari topik ta untuk semester ini , lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id” , judul TA apa yang dibuka oleh ishaq ?

### Jawab :
a. Masukkan wireshark filter expression “http.host == monta.if.its.ac.id” :
(gambar)
b. lalu klik paket no.576 sehingga muncul info tentang paket 576
c. lalu copy alamat http://monta.if.its.ac.id/index.php/topik/detailTopik/194
d. lalu buka alamat link tersebut di browser :
(gambar)
e. Maka judul TA yang dibuka Ishaq adalah “Evaluasi unjuk kerja User Space
FileSystem(FUSE)”

## Soal 3

### Filter sehingga wireshark hanya menampilkan paket yang menuju port 80!

### Jawab :
a. Buka file resource “soal3-6.pcapng”
b. Masukkan wireshark filter expression “tcp.dstport == 80” ke dalam display filter
c. Berikut tampilannya:
(gambar)

## Soal 4

### Filter sehingga wireshark hanya mengambil paket yang berasal dari port 21!

### Jawab :
a. Buka resource “Soal 3-6”
b. Masukkan wireshark filter expression “tcp.srcport ==21” ke dalam display filter
c. Berikut tampilannya:
(gambar)
