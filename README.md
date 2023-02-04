### Upload project 
Di web github, login dan create repository baru sesuai nama aplikasi Di komputer \
cd /var/www/html/aplikasi/ \
git init \
git remote add origin https://github.com/laodefardin/aplikasi.git \
git remote -v \
git add . \
git commit -m 'Upload pertama' \
git push -u origin master \
Masukkan username dan password github 

### Upload pembaharuan 
cd /var/www/html/aplikasi/ \
git status // bakal ditampilkan daftar file yg mengalami perubahan \
git add namafile.php // update 1 file ke server \
git commit // update semua file ke server \
git push origin master // masukkan username dan password \
git log // cek perubahan di log \

### Baca perubahan 
cd /var/www/html/aplikasi/ \
git log \

### Buat cabang aplikasi 
git checkout -b cabangAplikasi \
git branch // lihat daftar cabang repo \
git push --set-upstream origin cabangAplikasi // usulkan pull request ke master \
Buka web github/repo terima confirm pull request dan merge ke master \
Delete branch yg sudah disetujui kalau tidak diperlukan lagi \
git checkout master // kembali ke repo master \
git pull // tarik semua pembaharuan dari server \
git branch --delete cabangAplikasi \

### Kembali ke commit sebelumnya 
git reset kode_angka_commit \
git reset --hard // Untuk me-reset index dan bekerja dengan kondisi commit paling baru \

git status // untuk menampilkan daftar file yang berubah \
git clone // menyalin repository \
git merge // menggabungkan branch ke branch aktif \
git diff // untuk menampilkan semua conflict \
git diff <source-branch> <target-branch> // u/ menampilkan conflicts diantara branch yg akan di-merge \
git diff --base <nama-file> // Untuk melihat conflicts dengan file dasar \
git rebase master // untuk menerapkan ulang commit di branch yang lain \
git revert // Merevisi commit dengan git revert
