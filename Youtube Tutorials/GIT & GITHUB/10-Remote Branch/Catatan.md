### Remote Branch
Remote branch itu digunakan ketika kita ingin mengusulkan perubahan (pull request) kepada repo aslinya.

>> Sebaiknya branch Main/Master itu jangan di ubah, ketika kita ingin melakukan perubahan lebih baik membuat branch lalu melakukan merge

---
1. Masuk ke fork repository simple-landing-page
1. buat branch featurea, untuk membuat branch dan pindah ke branch yang dibuat bisa dengan command `git checkout -b <nama-branch>`
1. lakukan perubahan lalu commit
1. push ke origin dengan branch features `git push origin features`
1. lakukan pull request, untuk melakukan pull reques kita tidak bisa langsung dari git karena ini adalah feature dari github:
    1. masuk ke repo simple-landing-page
    1. pindah ke branch features
    ![screenshot](<Screenshot\Screenshot 2026-10-13 233040.png>)
    1. klik Contibute lalu klik open pull request
    ![](<Screenshot\Screenshot 2026-10-13 233636.png>)
    1. isikan pesan lalu klik create pull request

Sinkronkan dengan repo utama :
1. `git fetch sandhikagalih`
1. masuk ke branch master/main
1. `git merge sandhikagalih/master`
1. `git push origin master`
1. `git branch -d feature`
1. `git push origin --delete features`