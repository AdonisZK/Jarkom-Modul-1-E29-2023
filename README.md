# Jarkom-Modul-1-E29-2023

Laporan resmi pengerjaan soal praktikum Jarkom Modul 1 Kelompok E29 berupa dokumentasi dan screenshot output, cara pengerjaan, serta kendala yang dialami.

# Anggota Kelompok
| Nama | NRP |
| --- | --- |
| Sekar Ambar Arum | 5025211041 |
| Sony Hermawan | 5025211226 |

### No 1
**User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file.** <br />
+ a. Berapakah sequence number (raw) pada packet yang menunjukkan aktivitas tersebut? <br />
answer: 258040667 <br />
+ b. Berapakah acknowledge number (raw) pada packet yang menunjukkan aktivitas tersebut? <br />
answer: 1044861039 <br />
+ c. Berapakah sequence number (raw) pada packet yang menunjukkan response dari aktivitas tersebut? <br />
answer: 1044861039 <br />
+ d. Berapakah acknowledge number (raw) pada packet yang menunjukkan response dari aktivitas tersebut? <br />
answer: 258040696 <br />

![1 5](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/edbbeb05-c0db-4355-ada4-cc3ab05fd43f) <br />

**Penyelesaian**
- Melakukan filter ftp, kemudian mencari command STOR karena aktivitas yang dilakukan adalah mengunggah file.
  
  ![1 1](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/b02b6103-41a5-414e-9e59-76e8ac95d39f)

- Pada bagian Transmission Protocol Control, terdapat nilai sequence number (raw) dan acknowledge number (raw) dari aktivitas tersebut.
  
  ![1 2](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/e779fd26-7ab8-4146-9f13-a6c858887b5f)

- Untuk melihat nilai sequence number (raw) dan acknowledge number (raw) yang menunjukkan response dari aktivitas tersebut, melakukan TCP Stream.
  
  ![1 3](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/dacbf881-6f35-4bcc-8895-316a6f9d41de)

- Lalu, merujuk pada command setelah STOR.
  
  ![1 4](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/d94587c5-e86d-4b3f-a75b-03a98bbf5af6)

### No 2
**Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!** <br />
answer: gunicorn <br />

![2 4](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/8a078b41-9f9d-4f26-aac0-94919cbef183)

**Penyelesaian**
- Melakukan filter ip.addr == 10.21.78.111.
  
![2 1](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/22ba8796-1922-4ea9-bc21-818cce279cf1)

- Kemudian, pilih salah satu paket untuk dilakukan TCP Stream.
  
![2 2](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/a31f52c2-8dd3-4e28-b9cf-46a19dbcc893)

- Akan tampak server yang digunakan adalah gunicorn.
  
![2 3](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/ef85a7aa-950b-4350-9e06-b7637bed846c)

### No 3
**Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:**
+ a. Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702? <br />
answer: 21 <br />
+ b. Protokol layer transport apa yang digunakan? <br />
answer: UDP <br />

![3 4](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/1441e0cf-2fb2-4c1e-a64d-5e013e4e658e)

**Penyelesaian**
- Melakukan filter ip.addr == 239.255.255.250.

![3 1](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/692ff951-896a-4ad6-b3f5-5f311a93fa5c)

- Kemudian mencari paket dengan Dst port: 3702 dan menghitung jumlahnya yaitu 21 paket.

![3 2](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/748f143b-442a-4cff-a1f3-0ac43a147148)

- Protokol layer transport yang digunakan adalah UDP.

![3 3](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/c128d096-df23-472b-a2f4-af2b521d0899)
  
### No 4
**Berapa nilai checksum yang didapat dari header pada paket nomor 130?** <br />
answer: 0x18e5

![4 2](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/1262ec2d-399e-405c-aa9f-8716bfff15d2)

**Penyelesaian**
- Mencari paket nomor 130, kemudian melihat pada bagian User Datagram Protocol. Dapat ditemukan nilai checksum yaitu 0x18e5

![4 1](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/80a30b02-041f-4346-99bc-3eba113a7289)

### No 5
**Elshe menemukan suatu file packet capture yang menarik. Bantulah elshe untuk menganalisis file packet capture tersebut.**
+ a. Berapa banyak packet yang berhasil di capture dari file pcap tersebut? <br />
answer: 60 <br />
+ b. Port berapakah pada server yang digunakan untuk service SMTP? <br />
answer: 25 <br />
+ c. Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP? <br />
answer: 74.53.140.153 <br />

![5 6](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/59a34054-b906-4f6a-9f4b-572546126a0e)

**Penyelesaian**
- Melakukan filter smtp dan mencari paket yang mengandung password agar dapat membuka file zip.

![5 1](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/3e9f1988-e8f9-4284-9b73-c1bb3ed7075d)
  
- Lalu, decode password menggunakan base64 converter.

![5 2](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/2466c8e2-1609-4b4b-bdc9-d2788440a458)

- Kemudian, buka file zip untuk mendapatkan instance soal.

![5 3](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/4584093e-900f-4381-b5b9-ae7430476a23)
- Dengan begitu, soal yang ada dapat dikerjakan. Jumlah paketnya 60, port pada server yang digunakan untuk service SMTP adalah 25, dan public IP dari semua alamat IP yang tercapture adalah 74.53.140.153.

![5 4](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/616394d6-65b9-4605-b449-8f147b7cd113)

![5 5](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/e0955e11-9e82-48aa-8b8a-08d15770cb29)

### No 6
**Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut.** <br />
Kode Rahasia : SUBSTITUSI <br />
answer: JDRNJA <br />

**Penyelesaian**
Jika dilihat dari soal SOURCE ADDRESS 7812 maka kita melihat pada packet 7812

![image](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/48209612/23a03e41-b7f8-4cfb-b455-ca560b896cd0)

Jika dilihat dari IP source maka didapatkan 104.18.14.101. Jika dirubah menjadi alphabet seperti pada soal a1 e5 u21 maka 10(J) 4(D) 18(R) 14(N) 10(J) 1(A) <br />

**Kendala**  
Soal sedikit membingungkan membuat solver mengira bahwa answernya adalah SUBSTIUSI yang diubah menjadi numeric <br />

### No 7
**Berapa jumlah packet yang menuju IP 184.87.193.88?** <br />
answer: 6 <br />

**Penyelesaian**  
Melakukan filter ip.addr 184.87.193.88 lalu menghitung packet yang memiliki destination 184.87.193.88
Menghitung packet yang menuju IP 184.87.193.88 ada 6 

![image](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/48209612/6c6905cf-59a9-4895-a892-b70eab360f8e)

filter:  ip.addr == 184.87.193.88 

### No 8
**Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)**  <br />
answer: tcp.port == 80 || udp.port == 80

**Penyelesaian**  
Mengecek port melalui 2 jenis protocol yaitu tcp dan udp

![](https://lh6.googleusercontent.com/-tfUOH6vfAtgQj13UUP5aTflWd4KMREWiRAqWlOBgc698pMb0ttWcnd_Vj1y8aQ6vsxkwIgJHAXyh1Gi8YOgO4xjHFufxaldNlKc7-EUC8zR6gwyx5rp111TeH_BuftnOr1PLIy5shlqHpK0NAuGrqw)
Filter dan answer sama

Ref: https://osqa-ask.wireshark.org/questions/50586/capture-tcp-and-udp-packets-on-port-80/  <br />

### No 9
**Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!** <br />
answer: ip.src == 10.51.40.1 && ip.dst != 10.39.55.34 

**Penyelesaian** 
Melakukan filter dengan ip.src == (berasal) dan ip.dst != (tidak menuju)

![image](https://lh4.googleusercontent.com/Zq3AzXT32zd-Vu9pa0VCHUZ6HFG36cvTdlFyWZSdW1bNmoBtbeJMVgnRSdKlQ1KSVgEKTmEerkV5bjU2AEudpxiNP5usSQvJbO425FcZEF5veEvlGsu3TrlmyCYYIqyzscZQ2vDBMlSq2W6pV7FZNt4)

Filter dan answer sama

**Kendala** 
Banyak variasi yang dapat dilakukan untuk mengfilter seperti jawaban (contoh: ip.src == 10.51.40.1 and ip.dst != 10.39.55.34, ip.src eq 10.51.40.1 and !ip.dst == 10.39.55.34) dan pada saat awal praktikum jawaban tidak bisa walaupun sudah benar.

### No 10
**Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet**  <br />
answer: dhafin:kesayangannyak0k0

**Penyelesaian**
Dengan melakukan filter telnet pada packet 236 maka akan terlihat huruf per huruf untuk username dan password pada packet terakhir 262 atau bisa melakukan follow tcp stream
Filter: telnet

![](https://lh5.googleusercontent.com/zdJODhF-AKmz75X1MROZU1WBXMThSJUAf9qyPsHH8ttm6W-jz4jG2HZyM99EtQCoRTMzo0Hjt5n12FQ87Z-TyGBWm5OJEYP7D03StVN3yC7deiRO8zqIpR3n-m5ar62wNteDMoehwbjcprJbN15z1C0)

![](https://lh3.googleusercontent.com/JZjnrj63eUFtAWWbuYAhGmSfIQAmbzu0RkE_oCzr6ZIf0DH34CmPQ-eH8r4iP4-ZscBnv_xl9svRT4LPbAvyl-AHWbu8hqbRWXv0RZhBmkEHgV_FKuDudFCuJwM8ZNjh9CgsdVaoShvJzMVDyT2o5gg)
