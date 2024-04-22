# Git

- [Git Local](#git-local)
  - [Instalasi Git](#instalasi-git)
  - [Git Command](#git-command)
- [Git Remote](#git-remote)

## Git Local
## Instalasi Git
- download Git di https://git-scm.com/downloads

## Git Command
```
git init
git add <file(s)>
git status
git commit
git config
git branch
git help
```

Area pada repo Git
  - Workinf tree
  - Staging area
  - History

1.  git init
    - membuat forder menjadi repo git
2.  git config --global user.name "<your-username>"
    - memasukkan username, sebaiknya username sama dengan username GitHUb
3.  git config --global user.email "<your-email>"
    - - memasukkan email, sebaiknya email sama dengan username GitHUb
4.  git status
    - informasi perubahan pada repo git
5.  git add <nama_file> / git add .
    - memasukkan file ke Staging area
6.  git commit / git commit -m "<message>" / git commit -am "<mesage>"
    - menyimpan perubahan ke repo git
    - -am bisa digunakan untuk file yang modified tampa harus memasukkan ke Staging area (git add)
7.  git log / git log -3 / git log --<nama_file>
    - melihat semua log commit / 3 log terakhir / spesifik log pada file
8.  git checkout <5 digit pertama id commit> / git checkout <5 digit pertama id commit> --<namafile>
    - kembali ke commit tertentu untuk semua file / spesifik file tertentu 
9.  git branch
    - menampilkan daftar branch
10. git branch <nama_branch>
    - membuat branch baru
11. git log --all --decorate --oneline --graph
    - menampilkan visualisasi branch dalam bentuk visual
12. git checkout <nama_branch>
    - ganti branch
13. git merge <nama_branch>
    - menggabungkan branch yang aktif dengan branch baru
14. git branch --merged
    - untuk mengetahui branch mana yang sudah di merged
15. git branch -d <nama_branch>
    - menghapus branch
16. git branch -D <nama_branch>
    - menghapus branch walaupun belun di merged

## Git Remote

# Github to Local
17. git clone <url-https-github>
    - mengambil repo yang ada di github ke komputer lokal
    - ini digunakan ketika repo di github mau di hubungkan ke lokal
18. git remote
    - melihat nama remote
19. git remote -v
    - melihat lebih detail remote
20. git push
    - mengirim perubahan di lokal ke github

# Local to Github
21. git remote add <nama-remote(origin)> <url-https-github>
    - membuat remote baru
    - ini digunakan ketika repo di local mau di hubungkan dengan github
22. git push -u origin main
    - memasukkan kode yang dibuat di lokal ke github
23. git fetch
    - mengecek commit di remote sudah sampai mana
24. git pull
    - mengambil perubahan dari github ke lokal
25. git rebase <nama_branch>
    - hampir sama dengan merge
    - untuk mensejajarkan branch master
