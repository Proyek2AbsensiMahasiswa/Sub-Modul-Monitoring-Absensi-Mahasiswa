<h2 align="center"BAB I <br>PENDAHULUAN </h2>
<br>
<strong>1.1	Latar Belakang Masalah</strong>
<p align="justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Politeknik Pos Indonesia adalah sebuah kampus yang mempunyai 9 prodi salah satu di antaranya yaitu D4 Teknik Informatika. DIV Teknik Informatika Politeknik Pos Indonesia adalah sebuah program studi yang bergerak dalam IT yang di dalamnya terdapat 3 kelas untuk tingkat I, 4 kelas untuk tingkat II, 4 kelas untuk tingkat III dan 2 kelas untuk tingkat IV yang sedang menjalankan Internship (praktek kerja di perusahaan). Total mahasiswa DIV Teknik Informatika Politeknik Pos Indonesia yang aktif mengikuti perkuliahan di kampus kecuali mahasiswa tingkat IV mencapai kurang lebih 350 mahasiswa.
Dari jumlah mahasiswa DIV Teknik Informatika Politeknik Pos Indonesia tersebut dalam kegiatan absensi perkuliahan masih memanfaatkan kertas dan pena sebagai sarana absensi. Kertas absensi diestafetkan dari mahasiswa yang satu ke mahasiswa yang lainnya tanpa terjamin absensi yang diisikan sesuai dengan kenyataan atau ada yang memanipulasi absensi tersebut.
Dalam kegiatan absensi mahasiswa tentu harus diadakannya pengawasan yang ketat baik itu dari pihak kampus seperti wali dosen, prodi atau dari luar kampus seperti orang tua mahasiswa itu sendiri.  Sehingga ketiga pihak tersebut bisa mengontrol anak didiknya dalam kehadiran perkuliahan, sehingga jika mahasiswa banyak yang tidak hadir tanpa adanya keterangan, sakit atau ijin mereka semua bisa tahu bahkan bisa mengetahui anak didiknya jika mendapatkan SP (Surat Peringatan) 1, SP 2, SP 3 atau DO (drop out). <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Data absensi ini menjadi perhatian serius mengingat kehadiran mahasiswa menjadi salah satu tolak ukur aktivitas mahasiswa dalam proses perkuliahan. Kesulitan yang sering ditemui adalah pada saat akan melakukan rekapitulasi data. Berkas/dokumen absensi harus dikumpulkan kemudian dikalkulasi. Hal ini sangat merepotkan mengingat banyaknya mahasiswa yang terdistribusi dalam setiap kelas.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Berdasarkan data dan fakta yang diuraikan di atas, maka diperlukan suatu sistem yang dapat memberikan solusi pada permasalahan tersebut yaitu dengan membangun suatu aplikasi yaitu “Sistem Pengelolaan Data dan Monitoring Absensi pada Program Studi DIV Teknik Informatika Politeknik Pos Indonesia  Menggunakan Framework Code Igniter”.
<br>
<br>
<strong>1.2  Identifikasi Masalah</strong><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Berdasarkan latar belakang di atas maka permasalahan yang di hadapi pada kegiatan absensi mahasiswa program studi DIV Teknik Informatika Politeknik Pos Indonesia diantaranya yaitu : <br> 
1.  Kegiatan absensi mahasiswa masih manual dengan diestafetkannya kertas absensi sehingga kurang terjaminnya keaslian data.<br>
2.  Informasi tentang kehadiran mahasiswa selama perkuliahan tidak sampai kepada orang tua sehingga orang tua tidak tahu apakah anaknya masuk kuliah atau tidak. 
<br>
<br>
<strong>1.3	Tujuan</strong><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Tujuan yang ingin dicapai pada pembuatan aplikasi ini adalah: <br>
1.  Mengelola data absensi mahasiswa secara terkomputerisasi yang diinputkan langsung oleh dosen ke dalam sistem sehingga terjamin keaslian datanya.<br> 
2.  Informasi kehadiran perkuliahan mahasiswa bersifat terbuka untuk orang tua, prodi, wali dosen yang mempunyai hak untuk itu.
<br>
<br>
<strong>1.4	Ruang Lingkup</strong><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Adapun batasan masalah yang menjadi ruang lingkup pada pembuatan sistem ini antara lain :<br>
1.	Aplikasi ini berbasis website menggunakan framework codeigniter.<br>
2.	Untuk menjembatani antara backend dan frontend, sistem ini menggunakan web service dan dilengkapi keamanan berupa login untuk admin, wali dosen, prodi, orangtua/mahasiswa.<br> 
3.	Aplikasi ini hanya memuat absensi untuk mahasiswa DIV Teknik Informatika, tidak untuk dosen atau pegawai Politeknik Pos Indonesia.<br>
4.	Aplikasi ini digunakan oleh 4 macam user. Pertama yaitu admin yang mengelola sistem  dan yang kedua yaitu wali dosen, lalu yang ketiga yaitu prodi dan yang terakhir yaitu orangtua/mahasiswa.<br>
5.	Untuk user prodi dan orang tua/mahasiswa, mereka hanya bisa melihat absensi.<br> 
6.	Database yang digunakan adalah Mysql.<br>
7.	Untuk memonitoring absensi, orang tua bisa mengeceknya pada website yang telah disediakan dengan memasukan NPM dan password anaknya serta bisa menerima laporan SP melalaui SMS.<br>
8.  Tidak terhubung langsung dengan sistem penjadwalan perkuliahan.<br>
<br>
<br>
<strong>1.5	Sistematika Penulisan</strong><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Hal-hal yang akan dibahas dalam laporan proyek 1 ini meliputi:<br>
BAB I: tentang rincian alasan / latar belakang membuat sistem absensi mahasiswa, mengidentifikasi masalah yang berkaitan dengan absensi mahasiswa, tujuan membuat sistem absensi mahasiswa, ruang lingkup pembuatan sistem absensi mahasiswa serta sistematika yang akan dibahas dalam penulisan laporan proyek II ini dari mulai Bab I sampai dengan Bab V. <br>
BAB II: tentang landasan teori atau semi teori yang berkaitan dengan absensi mahasiswa dan mendukung objek proyek II tentang absensi mahasiswa antara lain tentang pengertiam sistem, pengertian absensi, pengertian monitoring absensi, penjelasan sekilas tentang program studi diploma IV teknik informatika, CodeIgniter, PHP, Database, XAMPP, Flowchart/Flowmap, UML, serta Metodelogi Pengembangan Aplikasi dengan Waterfall.<br>
BAB III: tentang analisa dan perancangan sistem absensi mahasiswa hingga menjadi sebuah informasi yang relevansi dari mulai analisis dari proses yang sedang berjalan (belum memakai sistem) meliputi analisis prosedur/flowmap proses yang sedang berjalan dan analisa dokumen yang digunakan, analisis proses system yang akan dibangun meliputi analisa kebutuhan aplikasi dan analisis kebutuhan perangkat lunak dan perangkat keras. Selain itu terkait dengan perancangan menggunakan UML, di dalamnya terdapat use case diagram, class diagram, sequence diagram, collaboration diagram, activity diagram, statechart diagram, component diagram, deployment diagram, struktur menu dan perancangan antar muka.<br>
BAB IV:tentang implementasi dan pengujian dari sistem absensi mahasiswa yang telah dibuat. Implementasi berupa sistem/aplikasi/alat yang dibuat dengan komponen-komponen pendukung berupa program, lingkungan implementasi, tampilan antar muka, petunjuk pemakaian dan petunjuk instalasi. Sedangkan untuk pengujian dibuat untuk mengetahui apakah sistem yang dibuat telah sesuai dengan rancangan atau belum yang di dalamnya terdapat lingkungan implementasi, pembahasan hasil implementasi dan pengujian dan hasil pengujian. <br>
BAB V: berisikan tentang penutup yang meliputi kesimpulan dari sistem absensi mahasiswa yang telah dibuat serta saran yang diajukan untuk melengkapi program aplikasi yang dibuat.<br>

</p>
