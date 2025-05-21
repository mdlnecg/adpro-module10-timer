# Tutorial 10 Pemrograman Lanjut: Timer
### Madeline Clairine Gultom - 2306207846 - ADPRO A

## Understanding How It Works
![alt text](img/image.png)

Pada gambar di atas, kita dapat melihat bahwa output yang dihasilkan adalah "howdy!" dan "done!" karena program sedang menjalani fungsi `async` yang akan dijalankan setelah pemanggilan `executor.run()`. 

Sedangkan pada ketika terdapat penambahan kode `println!("Madeline's Komputer: hey hey!");` setelah bagian `spawner.spawn(async {`, maka perintah print "hey hey!" tersebut akan dieksekusi terlebih dahulu karena potongan kode tersebut berada pada program utama di mana tidak perlu menunggu executor dijalankan terlebih dahulu. Setelah itu, barulah disusul dengan pemanggilan `executor.run()` dan menjalani perintah yang terdapat dalam fungsi `async` seperti pada gambar berikut.

![alt text](img/image-2.png)

