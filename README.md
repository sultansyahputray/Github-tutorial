# Github-tutorial

## Konfigurasi awal (username dan email) :
```bash
git config --global user.name (username github)
```
*`git config --global user.name sultansyahputray`*

```bash
- git config --global user.email (email github)
```
*`it config --global user.email hahahihi@gmail.com`*
<br>
<br>

## Clone repository :
```bash
git clone (ssh atau https dari repo yg mau di clone) 
```
*`git clone git@github.com:sultansyahputray/Github-tutorial.git`*
<br>
<br>

## Pembuatan branch :
pentingnya bekerja bada suatu branch yang berbeda agar meminimalisir terjadi conflict antar pengguna pada repo bersama.
### 1. membuat branch baru :
```bash
git checkout -b (nama branch)
```
*`git checkout -b branch`*

### 2. cek saat ini sedang berada pada branch apa 
```bash
git branch
```

### 3. switching branch
```bash
git switch (nama branch yang dituju)
```
*`git switch main`*

<img src="img/branch.png" alt="image" width=50%/>
<br>
<br>

## Menambahkan hasil kerja ke repo
### 1. menambahkan file yang telah diubah
```bash
git add (file apa yang selesai dikerjakan)
```
*`git add Readme.md`*<br> 
*`git add .`*

### 2. Menyimpan perubahan ke repo (checkpoint)
```bash
git commit -m "(pesan atau catatan)"
```
*`git commit -m "update Readme`*

### 3. Mengupload semua perubahan pada repo lokal ke repo github
```bash
git push origin (nama branch)
```
*`git push origin branch`*
<br>
<br>

## Merger branch
Merger atau menggabungkan file dari suatu branch ke dalam main membutuhkan perhatian dibeberapa hal, mulai dari apakah data yang mau kita merge sudah data yang terbaru, lalu format pesan commit, dll.

### Membuat suatu permintaan penggabungan antara branch dengan main (pull request)
- **Buka repository yang sedang dikerjakan** <br>
<img src="img/repo.png" alt="image" width=50%/> 

- **Click pada menu pull request** <br>
<img src="img/klik-pr.png" alt="image" width=50%/> 

- **Buat pull request baru** <br>
<img src="img/new-pr.png" alt="image" width=50%/> 

- **Setting base dari branch yang akan kita compare adalah main dan peng-comparenya adalah branch kita** <br>
<img src="img/compare.png" alt="image" width=50%/> 

- **Lakukan pengecekan final file yang akan di merge, bandingkan kondisi sebelum commit dan sesudah commit** <br>
<img src="img/final-check.png" alt="image" width=50%/> 

- **Creat pull request** <br>
<img src="img/pr.png" alt="image" width=50%/> 

- **Pastikan bahwa pesan commit sudah final dan sesuai dengan format** <br>
<img src="img/final-commit.png" alt="image" width=50%/> 

- **Jika sudah sesuai, lakukan rebase and merge** <br>
<img src="img/rebase-merge.png" alt="image" width=50%/> 
<br>
<br>

## Kondisi apabila terjadi conflict pada saat push ke repo atau merger
Terdapat beberap kasus dimana kita mendapati adanya conflict ketika ingin push ke github, berikut beberapa alternatif penyelesaiannya : <br>
<img src="img/conflict.png" alt="image" width=50%/> 

### 1. Melakukan clone ulang repo
Disini kita menggunakan cara tradisional dimana kita mem-backup terlebih dahulu file yang telah kita kerjakan, lalu kita copy perubahan file kita ke repo yang akan kita clone ulang.

- **Mem-backup file yang telah kita kerjakan ke folder lain**
- **Menghapus repo lama pada lokal kita**
- **Menghapus branch kita pada repo tersebut**
- **Melakukan clone ulang pada repo yang dimaksud**
```bash
git clone (alamat ssh file yang dimaksud)
```
- **Meng-input perubahan yang sebelumnya telah kita buat ke file clone yang baru**
- **Buat branch baru, lalu push ke branch tersebut. Cek dengan membuat suatu pull request, lalu perhatikan hal yang berubah antara file pada main dengan branch kita**
- **Apabila dirasa tidak ada conflict, lanjutkan dengan rebase and merge**
