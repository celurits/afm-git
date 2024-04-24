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

Membuat forder menjadi repo git
```
git init
```
memasukkan username, sebaiknya username sama dengan username GitHUb
```
git config --global user.name "<your-username>"
```
memasukkan email, sebaiknya email sama dengan username GitHUb
```
git config --global user.email "<your-email>"
```
informasi perubahan pada repo git
```
git status
```
memasukkan file ke Staging area
```
git add <nama_file> / git add .
```
menyimpan perubahan ke repo git. -am bisa digunakan untuk file yang modified tampa harus memasukkan ke Staging area (git add)
```
git commit / git commit -m "<message>" / git commit -am "<mesage>"
```
melihat semua log commit / 3 log terakhir / spesifik log pada file
```
git log / git log -3 / git log --<nama_file>
```
kembali ke commit tertentu untuk semua file / spesifik file tertentu
```
git checkout <5 digit pertama id commit> / git checkout <5 digit pertama id commit> --<namafile>
```
menampilkan daftar branch
```
git branch
```
membuat branch baru
```
git branch <nama_branch>
```
menampilkan visualisasi branch dalam bentuk visual
```
git log --all --decorate --oneline --graph
```
ganti branch
```
git checkout <nama_branch>
```
menggabungkan branch yang aktif dengan branch baru
```
git merge <nama_branch>
```
untuk mengetahui branch mana yang sudah di merged
```
git branch --merged
```
menghapus branch
```
git branch -d <nama_branch>
```

menghapus branch walaupun belun di merged
```
git branch -D <nama_branch>
```
## Git Remote

# Github to Local
mengambil repo yang ada di github ke komputer lokal
```
git clone <url-https-github>
```
melihat nama remote
```
git remote
```
melihat lebih detail remote
```
git remote -v
```
mengirim perubahan di lokal ke github
```
git push
```

# Local to Github
membuat remote baru
```
git remote add <nama-remote(origin)> <url-https-github>
```
memasukkan kode yang dibuat di lokal ke github
```
git push -u origin main
```
mengecek commit di remote sudah sampai mana
```
git fetch
```
mengambil perubahan dari github ke lokal
```
git pull
```
hampir sama dengan merge. untuk mensejajarkan branch master
```
git rebase <nama_branch>
```
