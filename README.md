# PRAKTEK GIT

## Inisialisasi GIT

```sh
$ git init
```

## Perubahan Sementara (Staging)

Menyimpan perubahan sementara dari working directory ke dalam staging area

```sh
$ git add <...dir_file>
$ git add <...dir_folder>
```

## Perubahan Permanen (Commit)

Menyimpan seluruh staging menjadi permanen, pesan commit berdasarkan [conventional commit](https://www.conventionalcommits.org/en/v1.0.0/), untuk tipe commit bisa mengacu ke [angular convention](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#type)

```sh
$ git commit
$ git commit -m "<pesan>"
```

## Pengecekan Status Working Directory

Bisa digunakan untuk melihat status baik yang sudah di staging area ataupun belum

```sh
$ git status
```

Bisa digunakan untuk melihat riwayat/history commit

```sh
$ git log
```

Bisa digunakan untuk melihat riwayat/history commit versi private
```sh
$ git reflog
```

## Manajemen Git Remote

```sh
$ git remote <command> <argument>
```

Digunakan untuk menghubungkan antara git yang di komputer lokal dengan git yang ada di penyedia layanan git (github, gitlab, dll.)

```sh
$ git remote add <alias_remote> <link_alamat_repo>
```

Digunakan untuk melihat list remote

```sh
$ git remote [-v]
```

Digunakan untuk melihat isi dari alias remote

```sh
$ git remote get-url <alias_remote>
```

## Synchronization

Digunakan untuk sinkronisasi dari lokal ke remote

```sh
$ git push [-u] <tujuan_remote> <branch_local>
```

Digunakan untuk sinkronisasi dari remote ke lokal

```sh
$ git pull <target_remote> <branch_remote>
```

## Copy Remote Repository to Local Computer

Digunakan untuk meng-kloning remote repo

```sh
$ git clone <link_remote> [<custom_name>]
```

Ketika di clone, link_remote langsung di set menjadi remote origin

## Undoing Changes

Konsep membalikkan waktu ke <span style="background-color: yellow;color:black">***id_commit***</span> tertentu untuk merubah history/riwayat git. <span style="background-color: yellow;color:black">***id_commit***</span> menjadi ***HEAD*** yang terbaru

```sh
$ git reset <id_commit>
```

Konsep yang menghilangkan history dengan <span style="background-color: yellow;color:black">***id_commit***</span> tertentu dengan history baru

```sh
$ git revert <id_commit>
```
