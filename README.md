# Tugas-Akhir-Pemos-Tim-5
Repositori ini dibuat untuk memenuhi Tugas Akhir Praktikum Pemodelan Oseanografi 2022. Repositori ini memuat teori, metode, analisis, dan file berupa script python (py) yang dapat memproses beberapa persamaan model seperti adveksi-difusi dan hidrodinamika 1D serta 2D untuk memodelkan suatu fenomena atau dinamika oseanografi.
# INSTALASI MINICONDA DAN LIBRARY 

## MODUL 1 ADVEKSI-DIFUSI 1D
### 1.1 TEORI DASAR
### 1.1.1 Adveksi 1D
  - Persamaan Adveksi Adalah salah satu persamaan diferensial parsial yang memodelkan pergerakan suatu konsentrat dalam cairan yang mengalir, dengan asumsi konsentrat tersebut tidak mengalami proses difusi di dalam cairan. adveksi berkaitan erat dengan aktivitas atau pergerakan suatu benda dari suatu tempat ke tempat lainnya untuk waktu tertentu. persamaan adveksi merupakan bentuk khusus dari persamaan diferensial untuk hukum kekekalan.
  - Persamaan umum Adveksi 1D:
  
  

- Dimana :
   F : Konsentrasi zat pelarut (mg/L)
   u : Kecepatan
   x : ruang sumbu horisontal (meter)
   t : waktu (detik)
- Metode Pendekatan dalam pemodelan numerik secara umum dibagi menjadi 2 pendekatan yaitu eksplisit dan implisit. metode eksplisit dibagi menjadi 3 yaitu:
- FTCS (Forward in Time Central in Space)
  Metode FTCS merupakan gabungan dari selisih maju terhadap waktu dan selisih pusat terhadap ruang. Solusi FTCS juga termasuk ke dalam solusi stabil bersyarat.
- Syarat kestabilan:
  

- Leapfrog (CTCS)
Metode beda hingga ini merupakan perluasan dari metode beda tengah (central difference) terhadap ruang dan waktu. Skema Leapfrog didapatkan dari turunan deret taylor, ini adalah skema konsisten. Leapfrog ini akan konsisten apabila nilai C ≤1.

![image](https://user-images.githubusercontent.com/105967489/169653369-2e0b4f94-18e2-474d-bdc4-715cadc843c0.png)


- Upstream
 Metode ini menggunakan pendekatan beda maju untuk turunan waktu, sedangkan untuk turunan terhadap ruang dilakukan dengan melihat arah kecepatan u. jika > 0 maka turunan terhadap menggunakan pendejatan beda mundur. Sebaliknya jika u < 0 maka digunakan pendekatan beda maju. Stabilitas metode upstream adalah sebagai berikut:
- Jika u > 0, turunan terhadap ruang menggunakan pendekatan beda mundur.
 ![image](https://user-images.githubusercontent.com/105967489/169652264-8bd6d155-a798-45e3-9796-25bc1bd43538.png)
- Jika u < 0, turunan terhadap ruang menggunakan pendekatan beda maju.
 ![image](https://user-images.githubusercontent.com/105967489/169652271-5894b538-197d-4d27-9498-ee546a24e993.png)

## 1.2 METODE

## MODUL 2 ADVEKSI-DIFUSI 2D
### 2.1 TEORI DASAR
- Adveksi merupakan mekanisme perpindahan massa suatu materi dari suatu titik ke titik lainya. Contoh adveksi adalah pengangkutan polutan atau endapan di sungai oleh aliran air curah ke hilir.
    Persamaan Adveksi 2D
![gambar](https://user-images.githubusercontent.com/105971274/169653219-816099ca-3c0a-4132-8c88-455223b7413b.png)
- Difusi adalah sebuah proses dimana suatu zat bergerak dari konsentrasi tinggi ke rendah, sehingga akan menghasilkan konsentrasi yang sama didalam zat tersebut.
    Persamaan Difusi 2D
![gambar](https://user-images.githubusercontent.com/105971274/169653265-89ac5ba3-74b0-4c69-ad2c-09dfb87c29ae.png)
- Pengaplikasian persamaan adveksi-difusi 2 dimensi digunakan sebagai pemodelan persebaran polutan. Persamaan adveksi-difusi 2D dapat digunakan juga dalam simulasi pergerakan atau persebaran tumpahan minyak (oil spill). Pengaplikasian persamaan adveksi difusi 2 dimensi digunakan untuk mengetahui distribusi partikel sedimen.

### 2.2 METODE
Metode deksritisasi model 2D pada bagian atau suku adveksi dan difusi umumnya menggunakan metode eksplisit upstream. 

- Adveksi 2D
Pada model adveksi 2D metode eksplisit upstream untuk Pada metode ini persamaan beda hingga menggunakan pendekatan beda maju untuk turunan waktu, dan untuk turunan terhadap ruang dengan melihat arah kecepatan u. Jika u>0 maka turunan terhadap ruang menggunankan pendekatan beda mundur. Jika u<0 digunakan pendekatan beda maju
    Persamaan dari metode diskritisasi untuk suku adveksi 2D
![gambar](https://user-images.githubusercontent.com/105971274/169654069-3e1a6646-352d-4755-acd3-8bcbafef31e0.png)

- Difusi 2D
Model 2D untuk mekanisme transpor difusi dapat menggunakan pendekatan beda maju untuk turunan waktu dan beda pusat untuk turunan ruang. Indeks n untuk waktu, indeks i untuk ruang, dan koefisiesn difusi AD dianggap konstan terhadap ruang dan waktu
    Persamaan diskritisasi untuk model 2D difusi adalah sebagai berikut
![gambar](https://user-images.githubusercontent.com/105971274/169654200-af9bf5b9-bc10-49fd-9af0-22a69f2f5447.png)

- Adveksi-Difusi 2D
Persamaan diskritisasi model 2D mendekati proses kejadian di alam. Untuk diskritisasi model 2D proses adveksi-difusi didapat dari menggabungkan deskritisasi dua suku yakni suku adveksi dan suku difusi. untuk model adveksi difusi 2D adalah sebagai berikut
![gambar](https://user-images.githubusercontent.com/105971274/169654760-cc46104a-fbbd-4ee2-9303-0139f48f283a.png)
### 2.3 SCRIPT DAN HASIL
### 2.4 ANALISIS

## MODUL 3 HIDRODINAMIKA 1D
### 3.1 TEORI DASAR
## 3.2 METODE
## 3.3 SCRIPT DAN HASIL
## 3.4 ANALISIS

## MODUL 4 HIDRODINAMIKA 2D
### 4.1 TEORI DASAR
### 4.2 METODE
1.	Buka miniconda lalu ketik jupyter notebook uuntuk membuka jupyter notebook sebagai text editor
 import matplotlib.pyplot as plt

from siphon.simplewebservice.ndbc import NDBC

df = NDBC.realtime_observations('51101')
df.head()

fig, (ax1, ax2, ax3) = plt.subplots(3, 1, figsize=(12, 10))
ax2b = ax2.twinx()

ax1.plot(df['time'], df['pressure'], color='darkorange')
ax1.set_ylabel('Pressure [hPa]')
fig.suptitle('Baiq Lista Azkia Sulhana_26050120120004_Ose A', fontsize=18)

ax2.plot(df['time'], df['wind_speed'], color='red')
ax2.plot(df['time'], df['wind_gust'], color='olive', linestyle='--')
ax2b.plot(df['time'], df['wind_direction'], color='mediumblue', linestyle='-')
ax2.set_ylabel('Wind Speed [m/s]')
ax2b.set_ylabel('Wind Direction')

ax3.plot(df['time'],df['water_temperature'], color='deepskyblue')
ax3.set_ylabel('Water Temperature [degC]')

plt.show()
2.	Tuliskan script diatas
![image](https://user-images.githubusercontent.com/96079752/169654713-e333bca4-b4a3-4c79-adeb-6137f3ed5877.png)

3.	Klik run untuk menjalankan script
![image](https://user-images.githubusercontent.com/96079752/169654727-a6cf7afa-53dc-4fe6-a2a7-f69a04521277.png)
 
4.	Setelah  menunggu beberapa saat akan muncul hasil seperti berikut
![image](https://user-images.githubusercontent.com/96079752/169654745-4c79b673-9abd-47d6-8848-ba6b7d40a387.png)
 
5.	Buka lama NDBC_NOAA untuk melihat lokasi station yang diperoleh sesuai NIM dan pada kolom Station ID Search ditulis ID lalu diklik Go
![image](https://user-images.githubusercontent.com/96079752/169654754-09359aff-d2ea-4023-b887-fe99ba8a9788.png)

6.	Maka akan muncul informasi mengenai lokasi stasiun sesuai ID yang dimasukkan seperti dibawah ini
![image](https://user-images.githubusercontent.com/96079752/169654775-7f4cd9b1-8efa-4780-aa25-cdbb2fce1749.png)
![image](https://user-images.githubusercontent.com/96079752/169654780-becab836-e8f2-4125-8ce8-febf62ba8936.png)


### 4.3 SCRIPT DAN HASIL

### 4.4 ANALISIS

## PENUTUP
