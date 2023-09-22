# Jarkom-Modul-1-E29-2023

Laporan resmi pengerjaan soal praktikum Jarkom Modul 1 Kelompok E29 berupa dokumentasi dan screenshot output, cara pengerjaan, serta kendala yang dialami.

# Anggota Kelompok
| Nama | NRP |
| --- | --- |
| Sekar Ambar Arum | 5025211041 |
| Sony Hermawan | 5025211226 |

### No 1
**User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file.** <br />
a. Berapakah sequence number (raw) pada packet yang menunjukkan aktivitas tersebut? <br />
answer: 258040667 <br />
b. Berapakah acknowledge number (raw) pada packet yang menunjukkan aktivitas tersebut? <br />
answer: 1044861039 <br />
c. Berapakah sequence number (raw) pada packet yang menunjukkan response dari aktivitas tersebut? <br />
answer: 1044861039 <br />
d. Berapakah acknowledge number (raw) pada packet yang menunjukkan response dari aktivitas tersebut? <br />
answer: 258040696 <br />

**Penyelesaian**
- Melakukan filter ftp, kemudian mencari command STOR karena aktivitas yang dilakukan adalah mengunggah file. <br />  
![1 1](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/b02b6103-41a5-414e-9e59-76e8ac95d39f)

- Pada bagian Transmission Protocol Control, terdapat nilai sequence number (raw) dan acknowledge number (raw) dari aktivitas tersebut. <br />
![1 2](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/e779fd26-7ab8-4146-9f13-a6c858887b5f)

- Untuk melihat nilai sequence number (raw) dan acknowledge number (raw) yang menunjukkan response dari aktivitas tersebut, melakukan TCP Stream. <br />
![1 3](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/dacbf881-6f35-4bcc-8895-316a6f9d41de)

- Lalu, merujuk pada command setelah STOR. <br />
![1 4](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/d94587c5-e86d-4b3f-a75b-03a98bbf5af6)

### No 2
**Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!**
- Melakukan filter ip.addr == 10.21.78.111. <br />
- Kemudian, pilih salah satu paket untuk dilakukan TCP Stream. <br />
- Akan tampak server yang digunakan adalah gunicorn. <br />
### No 3
### No 4
### No 5
### No 6
Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut. <br />
Kode Rahasia : SUBSTITUSI <br />
![image](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/48209612/23a03e41-b7f8-4cfb-b455-ca560b896cd0)

Jika dilihat dari IP source maka didapatkan 104.18.14.101. Jika dirubah menjadi alphabet seperti pada soal a1 e5 u21 maka 10(J) 4(D) 18(R) 14(N) 10(J) 1(A) <br />
Answer: JDRNJA

### No 7
### No 8
### No 9
### No 10
