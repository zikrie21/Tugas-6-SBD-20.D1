# TUGAS 6

- Nama : Zikri Hadiansyah
- Nim : 312010069
- Kelas : TI.20.D.1
- Matkul : Sistem Basis Data

# Soal

1. masuk ke database nama nim
2. lakukan proses backup dan recovery dengan sql
3. lakukan proses backup dan recovery dengan sqldump
4. tuliskan script cron job untuk melakukan backup otomatis setiap hari minggu jam 12 malam

# Jawaban

1. masuk ke database Zikri_312010069

![p](screenshot/ss1.png)

2. lakukan proses backup dan recovery dengan sql

- proses backup :
  ![p](screenshot/ss2.png)

- data backup terdapat pada file C:xampp\mysql\data\zikri_312010069
  ![p](screenshot/ss3.png)

- proses recovery :

* pertama hapus tabel yang telah dibackup dan mencoba menampilkan tabel
  ![p](screenshot/ss4.png)

* kemudian recovery tabel dan dicoba untuk menampilkan tabel
  ![p](screenshot/ss5.png)

3. lakukan proses backup dan recovery dengan sqldump

- proses backup :
  ![p](screenshot/ss6.png)

- proses recovery :
  ![p](screenshot/ss7.png)

![p](screenshot/ss8.png)

4. tuliskan script cron job untuk melakukan backup otomatis setiap hari minggu jam 12 malam

crontab –e

0 0 \* \* 7 myqldump -u root -p zikri_312010069 > mahasiswa_312010069_backupdata2.sql
