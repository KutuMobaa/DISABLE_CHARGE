# DISABLE_CHARGE


# CARA KERJA MODULE
- disaat module di flash, module akan membuat file `disable_charge` di directoty `/storage/emulated/0/Android` menggunakan `printf "80" > /storage/emulated/0/Android/disable_charge`. (angka `80` adalah nilai default batas maksimal battery melakukan pengecasan yang dapat di ubah sesuai keinginan ).
- setelah 7-10 detik device berhasil menyala, module akan membaca angka dari isi file `disable_charge` menggunakan `cat /storage/emulated/0/Android/disable_charge`.
- lalu module akan membandingkan nilai yang keluar dari file ` disable_charge` dengan level battery saat ini.
- 
 ***utama***
- jika level battery saati ini sama atau lebih besar dari nilai `disable_charge`, maka module akan membuat pengecasan otomatis berhenti.
- jika level battery saat ini lebih kecil dari nilai `disable_charge`, maka module akan membuat device dapat melakukan pengecasan secara normal.


**suport KSU ? We don't know yet.dwyor**
- `root only`
- *Download melalui telegram official untuk keaslian module dan gratis*

#
download module magisk di [Telegram](https://t.me/kutu_Moba57)
