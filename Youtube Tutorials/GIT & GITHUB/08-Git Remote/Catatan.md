# Git Remote
Remote adalah duplikat dari repo yang digunakan untuk menyingkronkan antara repo(yang berada di github) dan repo yang berada di lokal.

## Study case

### Dari github Cloning
1. buat repo baru di github
1. ketik `git clone https://github.com/rohmatHidayatYusuf/Rohmat-git-test.git`
1. ketik `git remote` digunakan untuk mengetahui remote
1. ketik `git remote -v` -v artinya verbose berguna untuk ketika kita ingin mengetahui data lebih detail.
1. ketik `git status` akan ada perbedaan saat kita tidak menggunakan remote "Your branch is up to date with 'origin/main'."
1. buat alias `alias graph="git log --all --decorate --oneline --graph"` panggil `graph` akan ada tiga branch yang berwarna merah itu adalah branch yang ada di remote kita.
1. tambahkan file index.html di repo lokal
1. lalu save dan commit perubahan. "Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)" artinya branch saat ini itu diatas branch yang ada di repo(github) jadi supaya sama ketik `git push`, untuk menghapus credensial gunakan credencial manager.

### Dari Lokal
1. buat folder baru `mkdir Rohmat-git-test2`
1. inisialisasi folder sebagai repo `git init`
1. buat repository di github tanpa menambahkan readme.md
1. tambahkan remote dengan mengetikan `git remote add origin https://github.com/rohmatHidayatYusuf/rohmat-git-test2.git`
1. ubah nama branch main `git branch -M main`
1. push repo lokal ke repo github `git push -u origin main` -u itu artinya upstream

### dilokal berubah di github berubah juga
1. tambahkan style.css di lokal dan tambahkan style.css di github lalu commit yang ada di github
1. lakukan commit yang ada di lokal
1. ketik `git pull` dan resolve koding.
