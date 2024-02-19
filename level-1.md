## Level 1: Back to basic

### Alur Pengerjaan

1. Inisialisasi git di local repo dan menghubungkan dengan remote repo

Dimulai dengan melakukan inisiasi menggunakan command `git init` pada working directory lalu membuat file README.md dan melakukan `git add` serta `git commit` pada local repo. Dilanjutkan dengan menciptakan remote repository baru dengan nama ajk-ricardo-penugasan1 sesuai dengan format, diakhiri dengan menjalankan `git add remote origin` untuk menghubungkan antara local repository dengan remote repository lalu melakukan push ke origin master. Serta menambahkan file baru untuk mencatat dokumentasi setiap level.

> Inisialisasi git pada local repository dan menghubungkan dengan remote repository

![Inisialisasi Git](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/1-fix.jpg>)

> Menciptakan repository baru di github

![New Remote Repository](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/1.5-fix.jpg>)

> Menambahkan dokumentasi untuk setiap level pada branch origin master

![Add level.md](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/2-fix.jpg>)

2. Membuat branch development serta menambahkan basecode (diselingi penerapan git reset)

Membuat branch development untuk menambahkan basecode lalu berpindah branch menggunakan `git checkout` dilanjutkan dengan menambahkan basecode di dalam file tersebut.

> Menambahkan branch baru dan menciptakan basecode

![Add branch development](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/3-fix.jpg>)

Saat memberikan pesan pada commit terdapat typo lalu melakukan `git reset` untuk membatalkan hasil commit yang telah dibuat. Serta melakukan restorasi menggunakan `git restore` untuk mengembalikan file sebelum di edit (tidak memberi efek apapun pada code di branch development karena tidak ada commit sebelumnya) dan memperbaharui message yang benar saat melakukan commit.

> Penggunaan git reset untuk membatalkan commit

![Git reset](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/4-fix.jpg>)

> Melakukan push ke origin development

![Push development (1)](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/5-fix.jpg>)

3. Menciptakan 2 branch _featureA_ dan _featureB_ untuk dilakukan conflict saat menjalankan perintah git merge

Membuat 2 branch baru untuk menambahkan fitur ke dalam basecode agar menciptakan conflict

> Membuat branch featureA dan featureB

![New branch](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/6-fix.jpg>)

Tetapi branch development ternyata membutuhkan tambahan untuk basecode, maka dari itu dilakukan penghapusan kedua branch tersebut menggunakan `git branch -d <nama-branch>`.

> Menghapus branch featureA dan featureB

![Delete branch](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/7-fix.jpg>)

Selanjutnya memberikan tambahan code pada basecode di branch development dan push ke origin development.

> Menambahkan basecode pada branch development

![Add basecode development](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/8-fix.jpg>)

4. Menambahkan fitur yang berbeda pada 2 branch tersebut (diselingi penerapan git stash)

Membuat 2 branch baru _featureA_ dan _featureB_ lalu berpindah di branch featureA untuk menambahkan code.

> Menambahkan fitur pada branch featureA

![Add fitur branch featureA](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/9-fix.jpg>)

Dikarenakan ingin melakukan implementasi `git stash` maka setelah menjalankan `git add .` dilanjutkan dengan menyimpan perubahan sementara menggunakan `git stash` untuk berpindah di branch featureB dan melakukan push fitur yang ditambahkan ke origin featureB.

> Penggunaan git stash dan push pada branch featureB

![Push featureB](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/10-fix.jpg>)

Kembali lagi ke branch featureA lalu menggunakan `git stash pop` untuk mengembalikan code yang tadi disimpan, lalu melakukan push ke origin featureA.

> Push pada branch featureA

![Push featureA](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/11-fix.jpg>)

5. Melakukan serta menyelesaikan conflict merge hasil merge --no-ff featureA ke development dilanjutkan featureB ke development

Setelah menambahkan kedua fitur tersebut selanjutnya berpindah ke branch development untuk melakukan git merge satu per satu dengan memanfaatkan `git merge --no-ff` untuk menciptakan conflict merge.

> Melakukan merge dari branch featureA dan featureB untuk menciptakan conflict

![Merge featureA](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/12-fix.jpg>)

> Hasil conflict yang terjadi

![Hasil conflict](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/13-fix.jpg>)

Conflict diselesaikan dengan menambahkan kedua merge tersebut secara bersamaan di branch development. Lalu melakukan push perubahan hasil merge tersebut di origin development.

> Push hasil merge di branch development

![Push development (2)](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/14-fix.jpg>)

Serta melakukan merge dari branch development ke branch master dan push ke origin master.

> Melakukan merge dari branch development ke branch master

![Merge ke branch master](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/15-fix.jpg>)

> Melakukan push ke remote repository

![Push origin master](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/15.5-fix.jpg>)

6. Menambahkan fitur pada branch development (untuk penerapan git diff)

Agar dapat mengimplementasikan `git diff` maka pada branch development ditambahkan feature baru dan menerapkan penggunaan `git diff` untuk mengetahui perbedaan yang terjadi sebelum dan sesudah meletakkan perubahan di staging area.

> Menambahkan fitur pada code di branch development

![Add fitur development](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/16-fix.jpg>)

> Implementasi penggunaan git diff

![Penggunaan git diff](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/17-fix.jpg>)

Dilanjutkan dengan melakukan push ke origin development, merge hasil perubahan ke branch master dan push ke origin master.

> Push origin development

![Push development (3)](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/18-fix.jpg>)

> Merge dan push pada branch master

![Merge and push master](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/19-fix.jpg>)

7. Menambahkan dokumentasi secara manual pada remote repo lalu melakukan git pull pada local repo

Mengimplementasikan `git pull` dengan melakukan commit pada branch master secara manual dari remote repository dan melakukan `git pull` pada branch master di local repository.

> mengganti pada github secara manual

![Commit github manual](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/20-fix.jpg>)

> Melakukan git pull

![Implementasi git pull](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/21-fix.jpg>)

### Dokumentasi Kondisi Git Graph

> Hasil dokumentasi Git Graph

![New Remote Repository](<https://github.com/Ricardo08S/ajk-ricardo-penugasan1/blob/master/src/img(level-1)/22-fix.jpg>)

### Keluh Kesah

- Saya mencoba beberapa menciptakan repo berbeda untuk eksperimen pake git dan mencari ide pembuatan alur yang mudah dan menerapkan semua perintah yang diminta
- Cukup menghabiskan waktu untuk ss sebagai bukti dokumentasi dan mengedit level-1.md
- masih ragu dengan keterangan singkat setelah konvensional message
