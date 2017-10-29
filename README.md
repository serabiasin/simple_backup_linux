# SIMPLE BACKUP LINUX
sangat cocok untuk orang yang malas melakukan copy-paster dari satu folder ke folder lain. Cukup melakukan mengatur folder/file yang ingin di backup , melakukan mounting external device (Flashdisk,Hard Disk external) dan mengatur direktori tempat untuk menampung backup.

## Pengaturan program <h2>

1.  pada Variable `from`, isi letak folder atau file yang ingin dibackup. 
2.  setelah itu pada variable `target`, masukkan direktori penyimpanan file yang di backup (jika ingin memindahkan ke media eksternal ikuti langkah berikut)
3. Cara Melakukan Mounting Media Eksternal
   1. pada terminal, `sudo fdisk -l`
   1. setelah itu akan muncul list penamaan partisi versi linux
   1. Biasanya untuk media eksternal, namanya adalah sdbX, X adalah nomor partisi
   1. Setelah mengetahui nomor partisi, membuat direktori sementara di /mnt/nama, "nama" bisa diganti sesuka anda perlu di ingat, folder ini yang akan di jadikan acuan variable `target`
   1. `sudo mkdir /mnt/nama`
   1. setelah itu ganti permissin dengan `sudo chmod -R -v 777 /mnt/nama/*`
   1. mount external drive dengan cara `sudo mount /dev/sdbX /mnt/nama`
   1.setelah itu lakukan eksekusi skrip tersebut

