## Nama : Ferzy Triwarsana Putra
## NIM : 2110131310003

# Komponen Sistem Operasi, Layanan Sistem Operasi  dan Sistem Call

## Komponen Sistem Operasi
<p align="justify">
Pada kenyataannya tidak semua sistem operasi mempunyai struktur yang sama. Namun menurut Avi Silberschatz, Peter Galvin, dan Greg Gagne, umumnya sebuah sistem operasi modern mempunyai komponen sebagai berikut:

Komponen Sistem Secara Umum

* Manajemen Proses
* Manajemen Memori Utama
* Manajemen File
* Manajemen Sistem I/O (input dan output)
* Manajemen Sekunder / Secondary
* Jaringan
* Sistem Proteksi
* Command-Interpreter Sistem

### Manajemen Proses
<p align="justify">
Proses adalah keadaan ketika sebuah program sedang dieksekusi. Sebuah proses membutuhkan beberapa sumber daya untuk menyelesaikan tugasnya. Sumber daya tersebut dapat berupa CPU time, memori, berkas-berkas, dan perangkat-perangkat I/O. Dalam hal manajemen proses, sistem operasi bertanggung jawab atas aktifitas-aktifitas yang berkaitan dengan manajemen proses seperti:

* Pembuatan dan penghapusan proses pengguna dan sistem proses
* Menunda atau melanjutkan proses
* nyediakan mekanisme untuk proses sinkronasi
* Menyediakan mekanisme untuk proses komunikasi
* Menyediakan mekanisme untuk penanganan deadblock

### Manajemen Memori Utama
<p align="justify">
Memori utama atau lebih dikenal sebagai RAM memori adalah sebuah array yang besar dari word atau byte, yang ukurannya mencapai ratusan, ribuan, atau bahkan jutaa. Setiap word atau byte mempunyai alamat tersendiri. Memori Utama berfungsi sebagai tempat penyimpanan yang akses datanya digunakan oleh CPU atau perangkat I/O. Memori utama termasuk tempat penyimpanan data yang sementara (volatile), artinya data akan hilang begitu sistem komputer dimatikan. Dalam hal manajemen memori, sistem operasi bertanggung jawab atas aktifitas-aktifitas yang berkaitan dengan manajemen memori seperti:

* Melacak bagian utama dari memori yang sedang digunakan & oleh siapa.
* Memutuskan proses-proses mana yang di-load ke ruang memori saat tersedia.
* Alokasi & dealokasi ruan memori.

### Manajemen Memori Sekunder
<p align="justify">
Karena memori utama (primary storage) bersifat volatile dan terlalu kecil untuk penyimpanan semua data dan program secara permanen, maka sistem komputer harus menyediakan secondnary storage untuk mem-backup memori utama. Sistem komputer modern menggunakan disk sebagai media on-line storage, yang digunakan untuk program dan data. Sistem operasi bertanggung jawab untuk aktifitas yang berhubungan dengan manajemen disk:

* Bagaimana mengelola ruang yang kosong dalam storage.
* Bagaimana mengalokasi storage.
* Bagaimana melakukan scheduling penggunaan disk.

### Manajemen File
<p align="justify">
File adalah kumpulan informasi yang berhubungan sesuai dengan tujuan pembuat file tersebut. File dapat mempunyai struktur yang bersifat hierarkis (direktori, volume, dll). Sistem operasi memberikan tanggapan atas manajemen file untuk aktifitas-aktifitas berikut:

* Pembuatan dan penghapusan file,
* Pembuatan dan penghapusan direktori,
* Mendukung primitif-primitif manipulasi file dan direktori,
* Pemetaan file dalam secondnary storage,
* Backup file dalam media yang stabil (non-volatile).

### Manajemen Input Output
<p align="justify">
Manajemen input output sering disebut device manager. Menyediakan "device driver" yang umum sehingga I/O dapat seragam (membuka membaca, menulis, menutup). Contoh: pengguna menggunakan operasiyang sama untuk membaca file pada hardisk, CD-ROM dan floppy disk.Sistem operasi memberikan tanggapan atas manajemen input-output untuk aktifitas-aktifitas berikut:

* Sistem buffer - caching: menampung sementara data dari I/O dan ke I/O
* Antarmuka device-driver secara umum atau spooling yang melakukan penjadwalan pemakaian  I/O supaya sistem lebih efisien  (seperti antrian pada proses)
* Driver untuk device hardware-hardware tertentu yang dapat melakukan operasi "detail" untuk perangkat I/O tertentu.

### Jaringan (Sistem Distribusi)
<p align="justify">
Sistem distribusi adalah kumpulan beberapa prosesoryang tidak membagi memori atau clock. Masing-masing prosesor mempunyai memori sendiri. Prosesor didalam sistem dihubungkan melalui suatu jaringan komunikasi dan komunikasi berlangsung dengan menggunakan suatu protocol. Sistem distribusi menyediakan akses user untuk berbagai sumber daya sistem. Akses terhadap sumber daya yang digunakan bersama mengizinkan:

* Mempercepat komputasi
* Peningkatan ketersediaan data
* Peningkatan keandalan

### Sistem Proteksi
<p align="justify">
Proteksi mengacu pada mekanisme untuk mengontrol akses yang dilakukan oleh program, prosesor, atau pengguna ke sistem sumber daya. Mekanisme proteksi harus:

* Membedakan antara penggunaan yang sudah diberi izin dan yang belum
* Menetapkan kontrol untuk diterapkan (spesify the controls to be imposed)
* Menyediakan tujuan dari pelaksanaan proteksi (provide a means of enforcement)

### Command-Interpreter System
<p align="justify">
Sistem operasi menunggu intruksi dari pengguna (command driven). Program yang membaca intruksi dan mengartikan control statements umumnya disebut: control-card interpreter, command line. Command interpreter memungkinkan sistem berkomunikasi dengan user melalui perintah-perintah menjalankan proses yang telah didefinisikan parameternya serta melakukan respon OS menunggu intruksi dari user (command driven).

<p align="justify">
Pada UNIX shell, command-interpreter System sangat bervariasi dari satu sistem operasi ke sistem operasi yang lain dan disesuaikan dengan tujuan dan teknologi I/O devices yang ada. Contohnya: CLI, Windows, Pen-based (touch), dan lain-lain.

<p align="justify">
Banyak perintah yang diberikan kepada sistem operasi oleh control statement yang berhubungan dengan:

* Process creation and management
* I/O handling
* Secondnary-storage management
* Main-memori management
* File-system access
* Protection
* Networking

## Layanan Sistem Operasi
<p align="justify">
Eksekusi program adalah kemampuan untuk "load" program ke memori dan menjalankan program. Operasi I/O: pengguna tidak dapat secara langsung mengakses sumber daya perangkat keras, sistem operasi harus menyediakan mekanisme untuk melakukan operasi I/O atas nama pengguna.

<p align="justify">
Sistem manipulasi file adalah kemampuan program untuk operasi pada file (membaca, menulis, membuat, dan menghapus berkas), Komunikasi adalah pertukaran data atau informasi antara dua atau lebih proses yang berada pada satu komputer atau lebih.

<p align="justify">
Sistem operasi memberikan pelayanan kepada programer sehingga pemrograman dapat dengan mudah dilakukan dalam hal sebagai berikut:

* Eksekusi program, sistem harus dapat memanggil program ke memori dan menjalankannya. Program tersebut harus dapat mengakhiri eksekusinya dalam bentuk normal atau abnormal (indikasi error),
* Operasi-operasi I/O, pada saat running program kemungkinan dibutuhkan I/O, mungkin berupa file atau peralatan I/O. Agar efisien dan aman, maka user tidak boleh mengontrol I/O secara langsung pengontrolan dilakukan oleh sistem operasi.
* Manipulasi sistem file. Kapabilitas program untuk membaca, menulis, membuat dan menghapus file.
Komunikasi, komunikasi dibutuhkan jika beberapa proses yang sedang dieksekusi saling bertukar informasi. Pertukaran informasi dapat dilakukan oleh beberapa proses dalam satu komputer atau didalam komputer yang berbeda melalui sistem jaringan. Komunikasi dilakukan dengan cara berbagi memori (shared memory) atau dengan cara pengiriman pesan (message passing).
* Mendeteksi kesalahan, sistem harus menjamin kebenaran dalam komputasi dengan melakukan pendeteksian error pada CPU dan memori, perangkat I/O atau pada user program.

<p align="justify">
Beberapa fungsi tambahan yang ada tidak digunakan untuk membantu user, tetapi lebih digunakan untuk menjamin operasi sistem yang efisien , yaitu:

* Mengalokasikan sumber daya (resource), sistem harus dapat mengalokasikan resource untuk banyak user atau banyak job yang dijalankan dalam waktu yang sama.
* Akutansi, sistem membuat catatan daftar berapa resorce yang digunakan user dan resource apa saja yang digunakan untuk menghitung statistik akumulasi penggunaan resource.
* Proteksi, sistem operasi harus menjamin bahwa semua akses ke resource terkontrol dengan baik.

## SISTEM CALL
<p align="justify">
Sistem call menyediakan penghubung (interface) antara proses menjalankan program dan sistem operasi, biasanya tersedia dalam bentuk intruksi bahasa assembly dan bahasa assembly digantikan untuk sistem programing agar mengizinkansistem call dibuat secara langsung. Ada sebelas langkah untuk membuat sistem call membaca (fd, buffer, nbytes), diantaranya adalah:

* Push nbyte
* Push dan buffer
* Pust fd
* Panggilan dibaca
* Meletakan code untuk dibaca oleh register
* Trap di kernel (dispatch)
* Masuk ke grap
* Sys call hardler
* Kembali ke posisi dipanggil
* Masuk ke increment SP
* Increment SP