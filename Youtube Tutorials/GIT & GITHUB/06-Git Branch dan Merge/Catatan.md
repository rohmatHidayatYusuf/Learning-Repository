# Git Branch dan Merge
Branch adalah cabang pada working tree yang digunakan ketika kita tidak yakin terhadap fitur baru yang ingin ditambahkan ataupun ingin bekerja dengan tim. Merge adalah penggabungan dua cabang.

## Implementasi Branch
Sebagai pendahuluan Git ketika kita membuat folder menjadi repo git akan membuatkan branch secara otomatis branch tersebut dinamakan master, untuk setiap commit yang dilakukan git akan menyimpan informasi seperti email account, timestamp, dan Hash commit. 
Hash commit yang disimpan oleh git akan terhubung dengan branch saat ini, untuk mengetahui branch saat ini ada teknik yang dinamakan head. Ketika kita melakukan perubahan dan melakukan commit pada perubahan tersebut maka pointer branch dan head akan berpindah ke Hash commit yang baru. command untuk menambahkan branch `git branch <nama branch>`, ketika kita menulis command tersebut tanpa mengisi nama branch cnth: `git branch` command tersebut akan menampilkan list branch.
Untuk melihat log commit biasa kita bisa tuliskan `git log` namun untuk melihat log dengan visualisasi graph kita bisa menuliskan `git log --all --decorate --oneline --graph` command tersebut nantinya akan terus digunakan, karena commandnya itu panjang kita bisa mempersingkat dengan cara menuliskan command berikut `alias graph="git log --all --decorate --oneline --graph"` alias adalah perintah dari shell
Untuk berpindah branch kita bisa menggunakan command ini `git checkout <nama branch>` command ini akan memindahkan pointer ke branch yang di tuju.

## Merging
`git merge <nama branch>`
`git merge <nama branch> -m "message"`
### Jenis Merge
- Fast forward merge
fast forward merge adalah merging yang langsung dilakukan saat branch nya itu direct path
- Three-way merge
Three-way merge dilakukan ketika tidak ada direct path 

## Menghapus branch
untuk menghapus branch kita bisa mengetikkan `git branch -d dosen`, untuk meyakinkan kita bisa mengetahui branch mana yang sudah di merge dengan command `git branch --merged`. Untuk menggunakan command ini `git branch -d dosen` kita sudah harus melakukan merge, untuk menghapus branch tanpa mempedulikan sudah di merge atau belum kita bisa menggunakan command ini `git branch -D dosen`
