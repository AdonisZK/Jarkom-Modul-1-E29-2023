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

**Penyelesaian**
![2 4](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/8a078b41-9f9d-4f26-aac0-94919cbef183)

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

**Penyelesaian**
- Melakukan filter ip.addr == 239.255.255.250.

![3 1](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/692ff951-896a-4ad6-b3f5-5f311a93fa5c)

- Kemudian mencari paket dengan Dst port: 3702 dan menghitung jumlahnya yaitu 21 paket.

![3 2](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/748f143b-442a-4cff-a1f3-0ac43a147148)

- Protokol layer transport yang digunakan adalah UDP.

![3 3](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/90591077/c128d096-df23-472b-a2f4-af2b521d0899)
  

### No 4
### No 5
### No 6
**Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut.** <br />
Kode Rahasia : SUBSTITUSI <br />
answer: JDRNJA <br />

**Penyelesaian**
![image](https://github.com/AdonisZK/Jarkom-Modul-1-E29-2023/assets/48209612/23a03e41-b7f8-4cfb-b455-ca560b896cd0)

Jika dilihat dari IP source maka didapatkan 104.18.14.101. Jika dirubah menjadi alphabet seperti pada soal a1 e5 u21 maka 10(J) 4(D) 18(R) 14(N) 10(J) 1(A) <br />

### No 7
### No 8
### No 9
### No 10
