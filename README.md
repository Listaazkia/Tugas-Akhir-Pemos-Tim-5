# Tugas-Akhir-Pemos-Tim-5
<p>Repositori ini dibuat untuk memenuhi Tugas Akhir Praktikum Pemodelan Oseanografi 2022. Repositori ini memuat teori, metode, analisis, dan file berupa script python (py) yang dapat memproses beberapa persamaan model seperti adveksi-difusi dan hidrodinamika 1D serta 2D untuk memodelkan suatu fenomena atau dinamika oseanografi.</p>

# AUTHORS
1. Baiq Lista Azkia Sulhana_26050120120004
2. Isti'anatul Khairat_26050120120023
3. Muhamad Asqi Rahmadani_26050120130066
4. Rieke Prameswina Legendevi_26050120140085
5. Syifa Fauziah_26050120130105
6. Gifbran Riki Pratama_26050120140156

# INSTALASI MINICONDA DAN LIBRARY 
1. Unduh Software pada link  [MINICONDA SOFTWARE](https://docs.conda.io/en/latest/miniconda.html#) dan pilih versi Windows dan Versi Python yang sesuaikan dengan jenis sistem operasi Windows yang digunakan.
2. File instalasi Miniconda dibuka dan pilih Run as administrator 
![image](https://user-images.githubusercontent.com/105970624/169655345-fdf61fa1-d32a-4ee1-b136-723fbf1b2613.png)
4. diklik "Next" pada Dialog Instalasi Minicond 
![image](https://user-images.githubusercontent.com/105970624/169655371-0bf27769-97e0-4c54-a9df-93e2ef0da71b.png)
6. diklik "I Agree" untuk Menyetujui Perjanjian Lisensi Software Miniconda 
![image](https://user-images.githubusercontent.com/105970624/169655415-fe953630-b98b-476a-a4a7-89ada23757eb.png)
8. dilakukan konfigurasi Instalasi Miniconda dan pilih "allUsers" 
![image](https://user-images.githubusercontent.com/105970624/169655444-83bf99bd-bb70-4d3f-8d5c-3fc06b641289.png)
10. Directory Penyimpanan Minicond dipilih 
![image](https://user-images.githubusercontent.com/105970624/169655480-7a93621e-e43d-4588-a05b-f8b9c60e0071.png)
12. Opsi Tingkat Lanjut Instalasi Miniconda "Register Miniconda as the system Python 3.9" untuk memperbolehkan IDE mengakses Python Environment Miniconda. lalu diklik install 
![image](https://user-images.githubusercontent.com/105970624/169655558-22471033-6e45-4e75-8f50-26ae46c874e1.png)
14. Tunggu Proses Instalasi 
![image](https://user-images.githubusercontent.com/105970624/169655567-c886d0bb-aa0b-4112-8601-0d82076cf6c6.png)
16. Klik "Finish" Dialog Instalasi Miniconda 
![image](https://user-images.githubusercontent.com/105970624/169655578-6e19407c-022a-4ca9-aa68-bfe7338dbd56.png)


# MODUL 1 ADVEKSI-DIFUSI 1D
# 1.1 TEORI DASAR
# 1.1.1 Adveksi 1D
*Persamaan Adveksi 
Persamaan Adveksi merupakan salah satu persamaan diferensial parsial yang memodelkan pergerakan suatu konsentrat dalam cairan yang mengalir, dengan asumsi konsentrat tersebut tidak mengalami proses difusi di dalam cairan. adveksi berkaitan erat dengan aktivitas atau pergerakan suatu benda dari suatu tempat ke tempat lainnya untuk waktu tertentu. persamaan adveksi merupakan bentuk khusus dari persamaan diferensial untuk hukum kekekalan.
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



# MODUL 2 ADVEKSI-DIFUSI 2D
# 2.1 TEORI DASAR
- Adveksi merupakan mekanisme perpindahan massa suatu materi dari suatu titik ke titik lainya. Contoh adveksi adalah pengangkutan polutan atau endapan di sungai oleh aliran air curah ke hilir.
- Persamaan Adveksi 2D

![gambar](https://user-images.githubusercontent.com/105971274/169653219-816099ca-3c0a-4132-8c88-455223b7413b.png)

- Difusi adalah sebuah proses dimana suatu zat bergerak dari konsentrasi tinggi ke rendah, sehingga akan menghasilkan konsentrasi yang sama didalam zat tersebut.
- Persamaan Difusi 2D

![gambar](https://user-images.githubusercontent.com/105971274/169666820-cc368012-44c2-4028-be8d-b4c89a71c9e7.png)

- Pengaplikasian persamaan adveksi-difusi 2 dimensi digunakan sebagai pemodelan persebaran polutan. Persamaan adveksi-difusi 2D dapat digunakan juga dalam simulasi pergerakan atau persebaran tumpahan minyak (oil spill). Pengaplikasian persamaan adveksi difusi 2 dimensi digunakan untuk mengetahui distribusi partikel sedimen

# 2.2 METODE
Metode deksritisasi model 2D pada bagian atau suku adveksi dan difusi umumnya menggunakan metode eksplisit upstream. 

- Adveksi 2D
- Pada model adveksi 2D metode eksplisit upstream untuk Pada metode ini persamaan beda hingga menggunakan pendekatan beda maju untuk turunan waktu, dan untuk turunan terhadap ruang dengan melihat arah kecepatan u. Jika u>0 maka turunan terhadap ruang menggunankan pendekatan beda mundur. Jika u<0 digunakan pendekatan beda maju
- Persamaan dari metode diskritisasi untuk suku adveksi 2D
![gambar](https://user-images.githubusercontent.com/105971274/169654069-3e1a6646-352d-4755-acd3-8bcbafef31e0.png)

- Difusi 2D
- Model 2D untuk mekanisme transpor difusi dapat menggunakan pendekatan beda maju untuk turunan waktu dan beda pusat untuk turunan ruang. Indeks n untuk waktu, indeks i untuk ruang, dan koefisiesn difusi AD dianggap konstan terhadap ruang dan waktu
- Persamaan diskritisasi untuk model 2D difusi adalah sebagai berikut
![gambar](https://user-images.githubusercontent.com/105971274/169654200-af9bf5b9-bc10-49fd-9af0-22a69f2f5447.png)

- Adveksi-Difusi 2D
Persamaan diskritisasi model 2D mendekati proses kejadian di alam. Untuk diskritisasi model 2D proses adveksi-difusi didapat dari menggabungkan deskritisasi dua suku yakni suku adveksi dan suku difusi. untuk model adveksi difusi 2D adalah sebagai berikut

![gambar](https://user-images.githubusercontent.com/105971274/169654760-cc46104a-fbbd-4ee2-9303-0139f48f283a.png)

# 2.3 SCRIPT DAN HASIL
# 2.4 ANALISIS

# MODUL 3 HIDRODINAMIKA 1D
# 3.1 TEORI DASAR
# 3.2 METODE
# 3.3 SCRIPT DAN HASIL
# 3.4 ANALISIS

## MODUL 4 HIDRODINAMIKA 2D
### 4.1 TEORI DASAR
<p> Hidrodinamika adalah cabang dari mekanika fluida, khususnya zat cair incompressible yang di pengaruhi oleh gaya internal dan eksternal (Cahyana, 2011). Dalam hidrodinamika laut gaya-gaya yang terpenting adalah gaya gravitasi, gaya gesekan, dan gaya coriolis. Dalam oseanografi, mekanika fluida digunakan  berdasarkan mekanika Newton yang dimodifikasi dengan memperhitungkan turbelensi</p>

- **Perbedaan Hidrodinamika 1D dan 2D**

### 4.2 METODE
1. Buka miniconda lalu ketik jupyter notebook uuntuk membuka jupyter notebook sebagai text editor 
![image](https://user-images.githubusercontent.com/96079752/169678825-36135327-8ced-43e9-b90c-18a646e41135.png)

*import matplotlib.pyplot as plt*
*from siphon.simplewebservice.ndbc import NDBC*

*df = NDBC.realtime_observations('51101') df.head()*

*fig, (ax1, ax2, ax3) = plt.subplots(3, 1, figsize=(12, 10)) ax2b = ax2.twinx()*

*ax1.plot(df['time'], df['pressure'], color='darkorange') ax1.set_ylabel('Pressure [hPa]') fig.suptitle('Pemodelan Hidrodinamika 2D_TIM 5', fontsize=18)*

*ax2.plot(df['time'], df['wind_speed'], color='red') ax2.plot(df['time'], df['wind_gust'], color='olive', linestyle='--') ax2b.plot(df['time'], df['wind_direction'], color='mediumblue', linestyle='-') ax2.set_ylabel('Wind Speed [m/s]') ax2b.set_ylabel('Wind Direction')*

*ax3.plot(df['time'],df['water_temperature'], color='deepskyblue') ax3.set_ylabel('Water Temperature [degC]')*

*plt.show()*

2. Tuliskan script diatas
![image](https://user-images.githubusercontent.com/96079752/169679102-7c744be3-1ab0-4a86-b54d-3b43e74f2b75.png)

3. Klik *run* untuk menjalankan script
![image](https://user-images.githubusercontent.com/96079752/169678800-38faec5f-e4d8-4f21-9d59-63566a4c9e63.png)

4. Setelah menunggu beberapa saat akan muncul hasil seperti berikut 
![image](https://user-images.githubusercontent.com/96079752/169678707-005fc3ab-874f-42a7-ac0b-e71022d8fff6.png)

5. Buka laman NDBC_NOAA untuk melihat lokasi station yang diperoleh sesuai NIM dan pada kolom Station ID Search ditulis ID lalu diklik Go
![image](https://user-images.githubusercontent.com/96079752/169678874-ae39ad63-8b14-43b0-9a9f-087b2a368a6c.png)

6. Maka akan muncul informasi mengenai lokasi stasiun sesuai ID yang dimasukkan seperti dibawah ini
![image](https://user-images.githubusercontent.com/96079752/169678878-5aa79921-c235-4d72-8cff-f4c6bdd6c8a6.png)
![image](https://user-images.githubusercontent.com/96079752/169678885-089fa6f5-7ce5-445f-a1f0-3e4447c78751.png)

### 4.3 SCRIPT DAN HASIL

- Script

![image](https://user-images.githubusercontent.com/96079752/169678930-1eaf03a8-27ec-40a7-80ee-5b2634f66112.png)

- Hasil
![image](https://user-images.githubusercontent.com/96079752/169678736-8e3cf07b-f508-48a5-b156-297fd3ba37ab.png)

### 4.4 ANALISIS
<p> Data parameter yang digunakan diantaranya tekanan, kecepatan angin, arah angin, dan temperatur air pada periode 5 minggu yaitu dari tanggal 15 maret 2022 sampai 22 april 2022. Grafik diatas diperoleh dari hasil ekstrak data NDBC (National Data Buoy Center) milik NOAA yang kemudian diplot-kan dalam bentuk grafik. Lokasi pengamatan yaitu di stastion ID 51101 yang berada di tengah samudra tepatnya di bagian samudra pasifik utara pada koordinat 24.361 N 162.075 W (24°21'40" N 162°4'30" W). Berdasarkan hasil diatas, terdapat 3 grafik dengan warna yang berbeda. Grafik pertama merupakan grafik tekanan, dari gambar tersebut tekanan di lokasi yang ditinjau menunjukkan nilai terendah sebesar 1012 hPa dan yang tertinggi 1025 hPa. Namun di setiap minggu nya grafik menggambarkan fluktuasi tekanan yang tidak konstan dimana tekanan cenderung naik turun dengan nilai terendah berada di akhir minggu pertama. Begitupula dengan grafik kecepatan angin dan arah angin yang menggambarkan fluktuasi naik turun dengan kecepatan angin tertinggi sebesar 13 m/s dan yang terendah sebesar 0,1 m/s. Arah angin berkisar di 30-100°, namun pada beberapa hari arah angin menunjukkan nilai yang tidak biasanya yaitu mencapai 320°. Hal ini mungkin bisa terjadi karena pada saat pencatatan data oleh buoy terjadi cuaca sehingga mempengaruhi pengukuran buoy di daerah tersebut yang mana membuat data arah pergerakan angin berbeda dari biasanya. Mengingat juga letak buoy yang berada di tengah samudra pasifik sangat memungkinkan untuk mendapat gangguan cuaca. Anomali yang terjadi ini dapat dikatakan hanyalah data error dan bukan siklon sebab menurut Ismail et al (2017), siklon tropis dapat terbentuk diatas lautan dengan suhu permukaan laut lebih dari 26˚C dan pada lintang kurang dari 5˚ siklon. Sedangkan dari data yang ada pada saat arah angin mencapai 320°, suhu permukaan laut tidak menghangat sampai nilai 26˚C, selain itu lokasi pencatatan tidak dilewati oleh siklon tropis. Untuk grafik ketika yaitu grafik temperatur yang digambarkan dengan warna biru langit menunjukkan fluktuasi yang tidak konstan dengan kisaran rat-rata berada di 24°C. Suhu tertinggi berada pada minggu pertama dengan nilai 25,2°C dan yang terendah terjadi pada minggu kedua dengan nilai 22,4°C. Dari grafik yang terlihat, suhu dan tekanan memiliki bentuk grafik yang berbanding terbalik, begitupula dengan suhu dan kecepatan angin. Artinya ketika suhu bernilai rendah, maka tekanan dan kecepatan angin tinggi. Sedangkan untuk hubungan tekanan dan kecepatan angin yaitu linier, sehingga bentuk grafik nya hampir sama. Tekanan udara pada permukaan bumi ditentukan oleh kerapatan massa udara. Makin rapat udara, tekanannya semakin tinggi. Kerapatan udara berhubungan erat dengan suhu, radiasi matahari, kelembaban dan gaya berat. Di suatu area dengan udara tipis, tekanan udara permukaan rendah. Di area dengan udara padat, tekanan di permukaan nya tinggi. Suhu dan tekanan sendiri memiliki hubungan yang terbalik dimana ketika suhu rendah maka tekanan tinggi disebabkan udara disana memiliki kerapatan massa yang tinggi. Sebaliknya, ketika daerah bersuhu tinggi maka tekanan udara diatasnya rendah karena kerapatan massa yang rendah. Perbedaan tekanan inilah yang selanjutnya membangkitkan pergerakan angin dan mempengaruhi kecepatan angin tersebut. Perbedaan tekanan udara pada daerah yang berbeda dengan ketinggian yang sama diakibatkan dari penerimaan radiasi matahari yang berbeda. Hal ini sejalan dengan Stewart (2008) yang menyatakan angin bergerak dari tekanan udara tinggi ke tekanan udara rendah dan kecepatan angin ditentukan oleh laju perubahan tekanan, dimana tekanan udara dapat mempengaruhi perubahan kecepatan angin. Besar kecil nya kecepatan angin ini akan berhubungan dengan tinggi gelombang yang dibangkitkan oleh angin, ketika kecepatan angin nya tinggi maka gelombang di daerah tersebut juga akan semakin tinggi.</p>
  
## PENUTUP
