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