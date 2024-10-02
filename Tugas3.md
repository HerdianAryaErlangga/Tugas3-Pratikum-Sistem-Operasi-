## Informasi Mahasiswa
**Nama: Herdian Arya Erlangga**\
**NIM: 09011182328099**\
**Kelas: SK3C**
<br>
<div align="Center">
  
### PRATIKUM 3 Sistem File (File System)
</div>



1. Lihat peralatan I/O, character device, yang ada pada system komputer.

jawab :

Disini saya menggunakan ls -l /dev untuk melihat semua alat-alat yang ada pada komputer saya
![1](https://github.com/user-attachments/assets/5dc8630a-9a90-45cb-a578-ed99075949fa)


2. Buatlah sub direktori januari, februari dan maret sekaligus pada direktori latihan5

jawab :

Menggunakan mkdir untuk membuat direktori
![2](https://github.com/user-attachments/assets/7f48d7c2-0cc3-4bdf-94be-e5d6cd1f64f5)


3. Buatlah file dataku yang berisi nama, nim dan alamat anda pada sub direktori januari
dan copy-kan file tersebut ke sub direktori februari dan maret.

jawab :

disini saya menggunakan nano untuk membuat file Dataku
![3](https://github.com/user-attachments/assets/826e6da3-7442-4d9c-8673-79dfe72312a2)
![3 1](https://github.com/user-attachments/assets/e659afbf-53a2-4f7e-b797-332dca8cce0c)


4. Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others 
dapat melakukan write. 

jawab :

disini saya menggunakan chmod tetapi tidak dengan go+w melainkan dengan angka yakni 666


g(group)o(other)+w(write), sedangkan untuk angka 


Read(r)=4


Write(w)=2


Execute(x)=1


yg dimana 666 (sesuai urutan angka pertama itu untuk user, kedua itu group, ketiga itu other)
disini itu 4(Read)+2(Write)=6(Read & Write)
![4](https://github.com/user-attachments/assets/5c5408cc-2ca3-4ed9-a9b9-b68b981e2de3)


5. Ubahlah ijin akses file dataku pada sub direktori pebruari sehingga user dapat 
melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read 
dan execute.


jawab :

![5](https://github.com/user-attachments/assets/fc56e45d-add6-4804-842e-f56232f46c0e)


6.  Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat 
melakukan write, read dan execute.

jawab :

![6](https://github.com/user-attachments/assets/eb69f21f-124a-4870-8e55-14b2bdaeb871)


7. Hapuslah direktori maret.

jawab :


disini saya tidak menggunakan rmdir karena rmdir hanya bisa menghapus direktori kosong, sedangkan direktori maret disini memiliki isi, jadi menggunakan rm -r maret
![7](https://github.com/user-attachments/assets/2ceec49d-25f1-4c33-b115-6d18c51f9dd0)


8. Ubahkan kepemilikan sub direktori februari sehingga user dan group hanya dapat 
melakukan read, dan cobalah untuk membuat direktori baru haha pada sub direktori 
februari.

jawab :


disini mengubah kepemilikan dir februari dengan chmod yg dmn itu user hanya dapat melakukan read saja dan itu berhasil dengan banyak nya akses saya yg ditolak, dan tidak bisa membuat dir haha
![8](https://github.com/user-attachments/assets/63fef44a-9fbb-4b5e-b715-d8c44aa63faa)


9. Modifikasi umask dari file dataku pada sub direktori januari menjadi 027 dan berapakan 
nilai default-nya ?

jawab :

umask default nya itu 0002, dan umask nya diganti ke 027, tetapi ini hanya berlaku untuk file dan dir baru, jadi untuk menyamakan file dataku menjadi umask 027(yg merubah izin default menjadi user rwx, group r-x, dan other tidak ada)
menggunakan chmod 750 Dataku
![9](https://github.com/user-attachments/assets/9df7a111-c66d-44a9-9c8b-ce3c8df76f97)


10.  Buatlah link dari file dataku ke file dataku.ini dan file dataku.juga dan dengan perintah 
list perhatikan berapa link yang terjadi ?

jawab :

disini saya menggunakan ln, dan bisa di lihat ada 3 link yg terjadi yg semua terhubung ke file dataku
![10](https://github.com/user-attachments/assets/7895fe8d-fd5b-44bd-b547-d390b3b7f662)
