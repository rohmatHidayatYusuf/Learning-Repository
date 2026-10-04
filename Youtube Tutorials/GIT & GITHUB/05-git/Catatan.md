# Git
Git menggunakan antarmuka command line interface (CLI) adapun git yang menggunakan graphical user interface (GUI) disebut git clien. Git dapat diinstall melalui wehsite resminya [link web](https://git-scm.com). Git juga menyediakan e-book mengenai bagaimana menggunakan git [Link E-book](https://git-scm.com/book/en/v2)

## Git Command local
- `$ git init`
digunakan untuk menginisialisasi folder menjadi repository
- `$ git add <file(s)>`
digunakan untuk menambahkan file ke dalam sesuatu yang disebut staging area
- `$ git status`
digunakan untuk mengetahui status pada repo kita
- `$ git commit`
digunakan untuk commit
- `$ git config`
digunakan untuk memasukan config ke dalam repo
-`$ git branch`
digunakan untuk membuat branch
- `$ git help`

## 3 Area pada Repo
- **Working Tree**
Working Tree adalah folder dimana kalian bekerja
- **Staging Area**
Staging area adalah pemberitahuan kepada git kalau kita melakukan perubahan
- **History**
History ini adalah proses yang nantinya perubahan yang kita lakukan itu akan di commit atau tidak

Staging area dan History nantinya akan tersimpan ke dalam folder .git. jadi folder .git ini akan muncul ketika kita sudah menginisialisasikan folder kita menjadi repository, dan untuk default folder nya ini akan tersembunyi

## Cara membuat Repo
1. buka git bash lalu masuk ke folder yang ingin kalian jadikan repo lalu ketikan `git init` setelah command tersebut diketikkan di bash akan muncul otomatis folder .git 
2. buat file index.html di dalam folder lalu ketik `git status` ini digunakan untuk apakah ada file yang belum di simpan ke stagging
3. ketik `git add <nama file>` untuk menyimpan file ke dalam stagging, anda bisa menghapus file dari stagging menggunakan command `git rm --cached <nama file>`
1. ketik `git config --global user.email "email@example.com"` lalu `git config --global user.name "Your Name"` 
1. lalu ketik `git commit -m "massage commit"` 
1. edit file index dan buat file baru bernama style.css lalu ketik `git status` di bash akan muncul untrack file dan changes not staged
1. untuk menambahkan semua file ke dalam stagging area kalian bisa ketik `git add .`
1. `git log` digunakan untuk melihat seluruh commit `git log -3` untuk melihat 3 commit terakhir `git log -- style.css` digunakan untuk melihat commit yang berkaitan dengan file style.css

untuk mengembalikan file yang sudah dihapus itu bisa menggunakan checkout caranya :
1. ketik `git checkout <5 digit commit code> -- <nama file>` itu digunakan untuk kembali ke commit sebelumnya tetapi hanya untuk file itu saja
