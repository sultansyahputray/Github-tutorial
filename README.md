# Github-tutorial

### Konfigurasi awal (username dan email) :
- git config --global user.name (username github) <br>
*git config --global user.name sultansyahputray*
- git config --global user.email (email github) <br>
*git config --global user.email hahahihi@gmail.com*

### Clone repository :
- git clone (ssh atau https dari repo yg mau di clone) <br>
<<<<<<< Updated upstream
*git clone git@github.com:sultansyahputray/Github-tutorial.git*
=======
*git clone git@github.com:sultansyahputray/Github-tutorial.git*

### Pembuatan branch :
pentingnya bekerja bada suatu branch yang berbeda agar meminimalisir terjadi conflict antar pengguna pada repo bersama.
1. membuat branch baru :
- git checkout -b (nama branch)
*git checkout -b branch*

2. cek saat ini sedang berada pada branch apa 
- git branch

3. switching branch
- git switch (nama branch yang dituju)
*git switch main*

<img src="img/branch.png" alt="image" width=50%/>

### Menambahkan hasil kerja ke repo
- git add (file apa yang selesai dikerjakan)
*git add Readme.md*
- git commit -m "(pesan atau catatan)"
*git commit -m "update Readme"
- git push origin (nama branch)
*git push origin branch*
>>>>>>> Stashed changes
