# Multiple Remote
kita akan melakukan fork tarhadap repo milik orang lain lalu akan dicopy ke github dan ke lokal

1. buka [github repository](https://github.com/sandhikagalih/simple-landing-page) lalu lakukan fork
1. cloning ke lokal komputer lalu masuk ke folder yang sudah di cloning
1. `git remote` `git remote -v` untuk mengecek remote itu punya sandhika atau milik rohmatHidayatYusuf
1. karena remote ini itu dari rohmatHidayatYusuf maka kita tidak tahu jiia repo sandhika update, untuk mengatasi itu kita bisa menambahkan remote baru yang mengarah ke repo sandhika dengan cara `git remote add sandhikagalih https://github.com/sandhikagalih/simple-landing-page`
1. `graph` disitu terlihat hanya ada dua remote yaitu master yang ada di lokal dan github, untuk melihat ke tiga branch harus dilakukan fetch terlebih dahulu `git fetch sandhikagalih`
studi kasus : repo sandhikagalih melakukan perubahan nah kita sebagai user yang fork repo sandhikagalih ingin mengetahui perubahan caranya
1. lakukan fetch ke remote shandikagalih `git fetch sandhikagalih`
1. lakukan merging `git merge sandhikagalih/master`
1. lakukan push ke remote origin atau github kita `git push -u origin master`