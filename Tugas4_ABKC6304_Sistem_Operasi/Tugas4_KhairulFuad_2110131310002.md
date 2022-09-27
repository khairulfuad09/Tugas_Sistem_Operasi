# Nama : Khairul Fuad
# Nim : 2110131310002

# Tugas 4

# Struktur Sistem Operasi

Struktur sistem operasi merupakan komponen-komponen sistem operasi yang dihubungkan dan dibentuk di dalam kernel. 

Sistem operasi sebagai kumpulan prosedur yang masing-masing dapat saling dipanggil jika dibutuhkan. Setiap prosedur yang ada di dalam sistem ini mempunyai interface yang sudah didefinisikan dengan baik.

Struktur tersebut adalah :

- Program utama yang meminta layanan prosedur.

- Kumpulan layanan prosedur yang membawa sistem call .

- Kumpulan utilitas prosedur yang membantu layanan prosedur.


## Mesin Virtual

Secara konsep, sistem computer dibuat berdasarkan lapisan. Hardware atau perangkat lunak merupakan tingkatan terbawah dari keseluruhan sistem. Kernel yang berjalan ditingkatan berikutnya menggunakan instruksi-intruksi perangkat keras untuk membuat kumpulan sistem call yang digunakan oleh lapisan luarnya. Program di atas kernel dapat menggunakan sistem call atau instruksi-instruksi perangkat keras. Dalam beberapa hal,program sistem tidak membedakan kedua lapisan tersebut.

## Struktur berlapis

Lapisan-lapisan sistem operasi adalah suatu abstraksi dari enkapsulasi sekumpulan struktur data dalam sistem operasi. Lapisan-lapisan yang berada di atas bisa mengakses operasi-operasi yang tersedia di lapisan-lapisan bawahnya.

- Lapisan 1. Berisi berbagai sirkuit elektronik, misal register, memory cells, dan logic gate.

- Lapisan 2. Berisi instruksi prosesor, misal instruksi aritmatika, instruksi transfer data, dsb.

- Lapisan 3. Penambahan konsep seperti prosedur/subrutin, maupun fungsi yang me-return nilai
tertentu.

- Lapisan 4. Penambahan interrupt.

- Lapisan 5. Program sebagai sekumpulan instruksi yang dijalankan oleh prosesor.

- Lapisan 6. Berhubungan dengan secondary storage device, yaitu membaca/menulis head, track,
dan sektor.

- Lapisan 7. Menciptakan alamat logika untuk proses. Mengatur hubungan antara main memory,
virtual memory, dan secondary memory.

- Lapisan 8. Program sebagai sekumpulan instruksi yang dijalankan oleh prosesor.

- Lapisan 9. Berhubungan dengan secondary storage device, yaitu membaca/menulis head,track,
dan sektor.

- Lapisan 10. Menciptakan alamat logika untuk proses. Mengatur hubungan antara main memory,
virtual memory, dan secondary memory.

- Lapisan 11. Program sebagai sekumpulan instruksi yang dijalankan oleh prosesor.

- Lapisan 12. File adalah objek yang memiliki nama dan ukuran. Abstraksi dari lapisan 9.

- Lapisan 13. Menyediakan interface agar bisa berinteraksi dengan pengguna

Lapisan-lapisan dari 1-4 bukanlah bagian dari sistem operasi dan masih menjadi bagian dari prosesor
secara ekslusif. Lapisan ke-5 hingga ke-7, sistem operasi sudah berhubungan dengan prosesor lapisan
ke-8 hingga 13, sistem operasi berhubungan dengan media penyimpanan maupun perlatan-peralatan
lain yang ditancapkan, misalnya peralatan jaringan.


## Mikro Kernel

Kernel merupakan program komputer yang menjadi inti dari sebuah sistem operasi komputer,dengan kontrol terhadap segala hal atas sistem tsb.

mikrokernel merupakan seperangkat perangkat lunak dalam jumlah minimum yang meyediakan beragam mekanisme dasar yang dibutuhkan untuk bekerja sebagai sebuah sistem operasi, mengeluarkan semua komponen yang tidak esensial.

fungsi utama mikro kernel adalah mendukung fasilitas komunikasi antar program client dan bermacam macam layanan secara tidak langsung oleh message-passing...tugasnya yaitu melayani bermacam macam program aplikasi untuk mengakses hardware secara aman.

contoh yang makai mikro kernel:
unix,TRU64 unix, macosX dan qnx

sebuah mikrokernel harus dapat meletakkan layanan-layanan sistem operasi pada tingkat yang paling atas

berikut adalah ruang fungsionalitas yang harus dimiliki mikrokernel

1. Sistem pengalamatan ruang dibtukan untuk mengatur proteksi ingatan

2. fungsi eksekusi secara abstrak untuk mengalokasi cpu yang biasanya adalah thread atau pengaktifan jadwal

3. komunikasi antar proses

kekurangan mikrokernel saat penambahan atau memodifikasi layanan memerlukan biaya tambahan dan bisa berimbas penurunan kinerja sistem.


