# DISABLE_CHARGE

# cara penggunaan
- flash
- reboot system
- edit file `status` ( jika kalian mau )
- enjoy.

# CARA KERJA MODULE
- disaat module di flash, module akan membuat file `status` di directoty `/storage/emulated/0/Android` dengan `printf "80" > /storage/emulated/0/Android/status`. angka `80` adalah nilai default batas maksimal battery melakukan pengecasan ( dapat di ubah sesuai keinginan ).
- setelah 7-10 detik device berhasil menyala, module akan membaca angka dari isi file `status` menggunakan `cat /storage/emulated/0/Android/status`.
- lalu module akan membandingkan nilai yang keluar dari file ` status` dengan level battery saat ini.
- 
 ***utama***
- jika level battery saati ini sama atau lebih besar dari nilai `status`, maka module akan membuat pengecasan otomatis berhenti.
- jika level battery saat ini lebih kecil dari nilai `status`, maka module akan membuat device dapat melakukan pengecasan secara normal.


**suport KSU ? We don't know yet.dwyor**
- `root only`
- *Download melalui telegram official untuk keaslian module dan gratis*
