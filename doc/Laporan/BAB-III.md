<h2 align="center">BAB III<br>
ANALISIS DAN PERANCANGAN</h2>
<br>
<p align="justify">
<strong>3.1   Analisis</strong><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Tahap analisis adalah tahap pemahaman terhadap suatu aplikasi yang telah dibuat. Dalam tahap ini bertujuan untuk mengetahui sistem dari aplikasi tersebut, proses-proses yang terlibat dalam aplikasi serta hubungan antar proses. Analisis juga sebagai penguraian atau penjelasan dari sebuah aplikasi yang utuh kedalam bagian-bagian komponennya dengan maksud untuk mengidentifikasi dan mengevaluasi masalah-masalah, kesempatan-kesempatan, hambatan-hambatan yang terjadi serta kebutuhan yang diharapkan sehingga terdapat usulan untuk perbaikan.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Analisis adalah langkah awal untuk pengembangan aplikasi, karena perancangan dan pengembangan implementasi aplikasi tidak akan berjalan dengan baik tanpa adanya analisa terhadap aplikasi yang akan digunakan. Analisis juga dapat didefinisikan sebagai penguraian dari suatu sistem informasi yang utuh kedalam bagian-bagian komponennya dengan tujuan serta maksud untuk mengidentifikasi dan mengevaluasi masalah-masalah, kesempatan-kesempatan, hambatan-hambatan yang terjadi serta kebutuhan- kebutuhan yang diharapkan sehingga dapat diusulkan recovery atau perbaikan.<br>
<br>
<b>3.1.1  Analisis Sistem yang Sedang Berjalan</b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Tahapan yang di perlukan dalam pembuatan suatu program yaitu menganalisa sistem yang telah ada, dimana analisa sistem merupakan proses mempelajari suatu sistem dengan cara menguraikan sistem tersebut kedalam elemen yang membentuknya. Selanjutnya mengidentifikasi dan mengevaluasi permasalahan – permasalahan yang terjadi serta kebutuhan yang di perlukan, sehingga dapat di susulkan pembuatannya.<br>
<br>
<b>3.1.1.1  Analisis Prosedur Berjalan</b><br>
<p align="center"><img src="../../img/Laporan/bpmn%20sedang%20berjalan.jpg" width="800" height="500">
<br>
Gambar 3.1 BPMN Absensi Mahasiswa Secara Manual <br></p>
Keterangan:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Untuk menguji model di atas, maka hal yang harus dilakukan yaitu memvalidasi simulasi yang diberikan durations 2 jam 30 menit 6 detik untuk melakukan aktifitas absensi secara manual, dari mulai penginputan absensi oleh dosen sampai menjadi laporan absensi mahasiswa. Di model tersebut digambarkan bahwa jika simulasi dimulai 450, maka output yang dihasilkan juga harus sama yaitu 450. Oleh karena itu, simulasi dari model absensi secara manual di atas telah valid. Pada simulasi tersebut dijelaskan bahwa semua task dan start/end even dari mulai menginputkan absensi sampai mengkalkulasikan absensi mahasiswa yang memuat laporan absensi berinstance complete 450, kecuali estafet absensi mahasiswa, proses pengecekan absensi dan gateway dimana proses tersebut akan terus berulang sampai kertas absensi mahasiswa terisi penuh, sehingga nilai instance complete yang didapat akan lebih dari 450 yaitu bernilai 902. Adapun hasil simulasi tersebut (result) adalah sebagai berikut:<br>
<p align="center"><img src="../../img/Laporan/Result%20informasi%20yang%20sedang%20berjalan.png" width="500" height="800">
<br> 
Gambar 3.2 Result BPMN Absensi Mahasiswa Secara Manual <br></p>
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Adapun dalam hal pemberitahuan kehadiran mahasiswa atau monitoring absensi mahasiswa pada proses yang sedang berjalan di Program Studi Diploma IV Teknik Informatika Politeknik Pos Indonesia saat ini tidak sampai secara langsung kepada orang tua. Pemberitahuan kehadiran hanya sampai pada mahasiswanya sendiri yang diberitahukan pada saat perwalian dengan dosen.<br>
<br>
<b>3.1.1.2  Analisis Dokumen yang Digunakan</b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Didalam proses absensi mahasiswa terdapat beberapa dokumen yang terlibat. Berikut ini adalah dokumen-dokumen yang dibutuhkan dalam sistem penjadwalan :<br>
<br>
Tabel 3.1 Data Prodi<br>
Dibuat oleh	    :	Admin<br>
Ditujukan untuk	:	Admin <br>
Isi	            :	prodi_kd, nama_prodi <br>
Tujuan	        :	Pengelolaan data prodi<br>
Frekuensi	    :	Fleksibel<br>
<br>
Tabel 3.2 Data Dosen<br>
Dibuat oleh	    :	Admin<br>
Ditujukan untuk	:	Admin & Operator<br>
Isi	            :	Dosen_kd, dosen_nama, dosen_alamat, dosen_email, dosen_status<br>
Tujuan	        :	Data mentahan untuk pembuatan jadwal<br>
Frekuensi	    :	Setahun sekali<br>
<br>
Tabel 3.3 Data Kelas<br>
Dibuat oleh	    :	Admin<br>
Ditujukan untuk	:	Admin<br>
Isi	            :	kd_kelas, nama_kelas<br>
Tujuan	        :	Untuk pengelolaan pembagian kelas<br>
Frekuensi	    :	Setahun sekali<br>
<br>
Tabel 3.4 Data Matakuliah<br>
Dibuat oleh	    :	Admin<br>
Ditujukan untuk	:	Admin & Operator<br>
Isi	            :	Matkul_kd, matkul_nama, matkul_jenis, matkul_sks, matkul_jam_teori, matkul_jam_praktek, matkul_total_jam, matkul_semester, matkul_thn_kurikulum, nama_prodi<br>
Tujuan	        :	Untuk pengelolaan mata kuliah dan data mentahan untuk pembuatan absensi.<br>
Frekuensi	    :	Enam bulan sekali <br>
<br>
Tabel 3.5 Data ruangan<br>
Dibuat oleh	    :	Operator<br>
Ditujukan untuk	:	Admin<br>
Isi	            :	Kd_ruangan, no_ruangan, lantai_ruangan, jns_ruangan, ruangan_status<br>
Tujuan	        :	Untuk pengelolaan ruangan kelas dan data mentahan untuk pembuatan absensi.<br>
Frekuensi	    :	Tidak ada patokan<br>
<br>
Tabel 3.6 Data Jadwal<br>
Dibuat oleh	    :	Admin & Operator<br>
Ditujukan untuk	:	Admin & Operator<br>
Isi	            :	Kd_jadwal, matakuliah, hari, kelas, dosen, jam, ruangan, prodi<br>
Tujuan	        :	Untuk pembuatan absensi<br>
Frekuensi	    :	6 bulan sekali<br>
<br>
Tabel 3.7 Data Absensi<br>
Dibuat oleh	    :	Admin & Operator<br>
Ditujukan untuk	:	Admin & Operator<br>
Isi	            :	Kd_absensi, tanggal, hari, kelas, matakuliah, jam, ruangan, keterangan kehadiran (hadir, sakit, ijin, alfa)<br>
Tujuan	        :	Untuk mengelola data absensi<br>
Frekuensi	    :	Fleksibel<br>
<br>
Tabel 3.8 Data Kelompok<br>
Dibuat oleh	    :	Admin<br>
Ditujukan untuk	:	Admin<br>
Isi	            :	Admin_level_kode, admin_level_nama, admin_level_status<br>
Tujuan	        :	Untuk mengelompokan pengguna/actor<br>
Frekuensi	    :	Fleksibel<br>
<br>
Tabel 3.9 Data Mahasiswa<br>
Dibuat oleh	    :	Admin<br>
Ditujukan untuk	:	Admin<br>
Isi	            :	Npm, nama mahasiswa, alamat mahasiswa, no hp mahasiswa, nama orangtua/wali, notelp orang tua/wali, alamat orangtua/wali,<br>
Tujuan	        :	Untuk mengelola data mahasiswa<br>
Frekuensi	     :	Fleksibel<br>
<br>
Tabel 3.10 Data Pelanggaran<br>
Dibuat oleh	    :	Admin<br>
Ditujukan untuk	:	Admin, Mahasiswa/ortu, dosen<br>
Isi	            :	Pelanggaran id, jenis pelanggaran, point<br>
Tujuan	        :	Untuk menentukan mahasiswa mendapatkan pelanggaran seperti SP1,SP2,SP3 atau dropout<br>
Frekuensi	    :	Fleksibel<br>
<br>
<b>3.1.2  Analisis Sistem yang akan Dibangun</b><br>
<b>3.1.2.1  Analisis Prosedur yang akan dibangun</b><br>
<p align="center"><img src="../../img/Laporan/bpmn%20dibangun%20sms.JPG" width="800" height="500">
<br>
Gambar 3.3 BPMN Monitoring Absensi Mahasiswa via sms<br></p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Adapun sub proses dari proses login pada BPMN Monitoring Absensi Mahasiswa via sms adalah sebagai berikut:<br>
<p align="center"><img src="../../img/Laporan/bpmn%20login.JPG" width="400" height="200">
<br> 
Gambar 3.4 BPMN Sub Proses Login<br></p>
Keterangan:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Pada model gambar 3.3, salah satu proses tersebut memeliki sub proses yaitu login, yang dijelaskan pada gambar 3.4. Untuk menguji model di atas, maka hal yang harus dilakukan yaitu memvalidasi simulasi yang diberikan durations 50 menit untuk melakukan monitoring absensi mahasiswa via sms, dari mulai penginputan absensi oleh dosen sampai orang tua menerima info pelanggaran melalui sms atau tidak mendapatkan sms info pelanggaran. Di model tersebut digambarkan bahwa jika simulasi dimulai 450, maka output yang dihasilkan juga harus sama yaitu 450, yaitu 158 yang tidak menerima sms info pelanggaran, dan 292 menerima sms info pelanggaran dengan list 147 mendapat SP1, 72 mendapat SP2 dan 73 mendapat SP3. Oleh karena itu, simulasi dari model monitoring absensi mahasiswa via sms di atas telah valid. Adapun hasil simulasi tersebut (result) adalah sebagai berikut:<br>
<p align="center"><img src="../../img/Laporan/result%20sms.JPG" width="500" height="800">
<br> 
Gambar 3.5 Result BPMN Monitoring Absensi Mahasiswa via sms<br>
<img src="../../img/Laporan/bpmn%20dibangun%20web.JPG" width="800" height="500">
<br> 
Gambar 3.6 BPMN Monitoring Absensi Mahasiswa via web<br></p>

Keterangan:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Untuk menguji model di atas, maka hal yang harus dilakukan yaitu memvalidasi simulasi yang diberikan durations 50 menit untuk melakukan aktifitas absensi secara manual, dari mulai login oleh mahasiswa atau orangtua sampai display abesensi mahasiswa. Di model tersebut digambarkan bahwa jika simulasi dimulai 450, maka output yang dihasilkan juga harus sama yaitu 450. Oleh karena itu, simulasi dari model absensi secara manual di atas telah valid. Pada simulasi tersebut dijelaskan bahwa semua task dan start/end even dari mulai mulai login oleh mahasiswa atau orangtua sampai display abesensi mahasiswa berinstance complete 450, kecuali input npm dan password, kelola login dan gateway dimana proses tersebut akan terus berulang sampai npm dan password yang diinputkan dinyatakan valid oleh sistem, sehingga nilai instance complete yang didapat akan lebih dari 450 yaitu bernilai 880. Adapun hasil simulasi tersebut (result) adalah sebagai berikut:<br>
<p align="center"><img src="../../img/Laporan/result%20web.JPG" width="600" height="800">
<br> 
Gambar 3.7 Result BPMN Monitoring Absensi Mahasiswa via web<br></p>
<br>
<b>3.1.2.2  Analisis Kebutuhan Aplikasi</b><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Kebutuhan fungsional dari sistem monitoring absensi mahasiswa adalah sebagai berikut:<br>
1.	Proses Monitoring Absensi Mahasiswa via sms<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Pada proses absensi yang berjalan sekarang di Program Studi D4 Teknik Informatika Politeknik Pos Indonesia belum terbuka untuk orangtua. Jika mahasiswa mendapatkan pelanggaran, pemberitahuannya hanya sampai kepada mahasiswa sendiri melalui dosen. Jadi, orang tau tidak tahu apabila anaknya betul betul hadir dalam perkuliahan atau sebaliknya.<br>
Untuk itu, proses monitoring absensi mahasiswa sangatlah penting, guna untuk mengontrol kehadiran mahasiswa. Adapun salah satu cara untuk memonitoringnya yaitu melalui sms. Jadi sistem akan mengirikan sms kepada orangtua apabila anaknya mendapatkan pelanggaran terkait absensi perkuliahan yaitu berupa SP1, SP2, SP3 atau dropout. Adapun yang menerima sms ini hanya orang tua mahasiswa, yang dikirimkan oleh admin atau BAAK melalui sistem.<br>
2.	Proses View Absensi Mahasiswa<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Pada proses absensi yang sedang berjalan saat ini di Prodi D4 Tenik Infomatika Politeknik Pos Indonesia, mahasiswa tidak bisa melihat absensi dirinya sendiri di web. Apabila mahasiswa ingin melihat absensinya, beliau harus datang ke prodi atau BAAK untuk melihat absensinya. Oleh karena itu, dengan sistem yang akan dibuat nanti, mahasiswa bisa melihat absensinya dengan memasukan username dan password (login) di web absensi nanti. Adapun yang dapat melihat absensi ini semua jenis user bisa melihatnya seperti BAAK, dosen, orangtua atau mahasiswa.<br>
<br>
<b>2.1.2.3	Analisis Kebutuhan Perangkat Lunak dan Perangkat Keras</b><br>
1)	Perangkat Lunak yang digunakan untuk membuat aplikasi ini meliputi:<br>
a.	Sistem Operasi	    : Windows 10 pro.<br>
b.	Editor Teks	        : Bracket.<br>
c.	Editor Grafik	    : Photoshop, Paint. <br>
d.	Web script language	:HTML,Javascript dan PHP Framework.<br>
e.	Database server	    : MySQL.<br>
f.	Client Application	: Google Chrome<br>	
<br>
2)	Perangkat Keras minimal yang digunakan untuk membuat aplikasi ini<br>
a.	untuk server meliputi:<br>
1)	Processor Intel Core i3<br>
2)	Memory  2 GB.<br>
3)	Harddisk 300 GB.<br>
4)	Modem Online Manager<br>
b.	untuk User  meliputi:<br>
1)	Processor Intel Dual Core<br>
2)	Memory  1 GB.<br>
3)	Harddisk 300 GB.<br>
</p>