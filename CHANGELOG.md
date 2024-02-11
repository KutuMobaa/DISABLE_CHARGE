# DISABLE_CHARGE V 5.8

# default
- menghentikan pengecasan di saat level battery mencapai 80% dan kembali melakukan pengecasan ketika level battery 79%.
- *default :*
  ![alt text](https://github.com/KutuMobaa/DISABLE_CHARGE/blob/main/Screenshot_20240210-041738146.jpg?raw=true)
# setting
- masuk ke directory `/storage/emulated/0/Android` lalu cari file bernama `status`, edit file tersebut dengan cara ubah angka sesuai keinginan kalian.
- *contoh :*
![alt text](https://github.com/KutuMobaa/DISABLE_CHARGE/blob/main/Screenshot_20240210-041817242.jpg?raw=true)

# cara penggunaan
- flash
- reboot system
- edit file `status` ( jika kalian mau )
- enjoy.

# CARA KERJA MODULE
- disaat module di flash, module akan membuat file `status` di directoty `/storage/emulated/0/Android` menggunakan `printf "80" > /storage/emulated/0/Android/status`. (angka `80` adalah nilai default batas maksimal battery melakukan pengecasan yang dapat di ubah sesuai keinginan ).
- setelah 7-10 detik device berhasil menyala, module akan membaca angka dari isi file `status` menggunakan `cat /storage/emulated/0/Android/status`.
- lalu module akan membandingkan nilai yang keluar dari file ` status` dengan level battery saat ini.
- 
 ***utama***
- jika level battery saati ini sama atau lebih besar dari nilai `status`, maka module akan membuat pengecasan otomatis berhenti.
- jika level battery saat ini lebih kecil dari nilai `status`, maka module akan membuat device dapat melakukan pengecasan secara normal.


**suport KSU ? We don't know yet.dwyor**
- `root only`
- *Download melalui telegram official untuk keaslian module dan gratis*

#
#
#
#
# DISABLE_CHARGE V 5.7

# default
- menghentikan pengecasan di saat level battery mencapai 80% dan kembali melakukan pengecasan ketika level battery 79%.
- *default :*
  ![alt text](https://github.com/KutuMobaa/DISABLE_CHARGE/blob/main/Screenshot_20240210-041738146.jpg?raw=true)
# setting
- masuk ke directory `/storage/emulated/0/Android` lalu cari file bernama `status`, edit file tersebut dengan cara ubah angka sesuai keinginan kalian.
- *contoh :*
![alt text](https://github.com/KutuMobaa/DISABLE_CHARGE/blob/main/Screenshot_20240210-041817242.jpg?raw=true)

# cara penggunaan
- flash
- reboot system
- edit file `status` ( jika kalian mau )
- enjoy.


![alt text](https://github.com/KutuMobaa/DISABLE_CHARGE/blob/main/Screenshot_20240210-014203823.jpg?raw=true)


- suport KSU ? We don't know yet.dwyor
- `root only`
- *Download melalui telegram official untuk keaslian module dan gratis*



# tambahan
- ***jangan pernah merubah file `status` selain angka.
- jika file `status` tidak ada di `/storage/emulated/0/Android`, buat manual dengan isi `enable=80`
- `Module ini masih tahap beta, jadi jika tidak bekerja di device anda silahkan hapus module lalu reboot system`
