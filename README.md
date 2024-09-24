<h2>
Nama : Rosmalinda <br/>
Nim : 09011282328086 <br/>
Kelas : SK3B
<h2/>

## 1. Eksekusi seluruh profile yang ada :
  **a. Edit file profile /etc/profile dan tampilkan pesan sebagai berikut :**                                   
       echo “Profile dari /etc/profile” <p/>
       <img src="https://github.com/user-attachments/assets/9e8d511e-f3d0-44db-8f9b-a93484ea3458" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/c0a5b5eb-ff13-4b0b-9c29-e09740c12116" width=500/>
       <br/>

  **b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :** 
    <p> Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap file tersebut, cantumkan instruksi echo,              misalnya pada /home/ mahasiswa/.bash_profile : 
       echo “Profile dari .bash_profile”
       Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang bersangkutan.<p/>
       **/home/stD02001/.bash_profile** <p/>
       <img src="https://github.com/user-attachments/assets/41cad3ba-f31c-49f2-a4bc-f7c08f9016f1" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/801caa14-7ac1-412c-b5ab-142acd738019" width=500/>
       <br/>
       **/home/. stD02001/.bash_login** <p/>
       <img src="https://github.com/user-attachments/assets/65125f01-1d00-4422-8df9-1f96627b6e4d" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/f15aa1f9-4b2b-429a-9333-a95dd6cb9f9a" width=500/>
       <br/>
       **/home/mahasiswa/.profile** <p/>
       <img src="https://github.com/user-attachments/assets/42437dca-3e11-481c-9e6c-31e31b4a78e0" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/731fb07f-770e-4b2d-8604-63f76ac4f851" width=500/>
       <br/>
       **/home/mahasiswa/.bashrc** <p/>
       <img src="https://github.com/user-attachments/assets/af8a89a5-8d4e-4cba-a5e0-84ca642d43ed" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/7e6a9d69-858d-4a05-9342-f3ddabb4a110" width=500/>
       <br/>
       
  **c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:** <br/>
       $ su mahasiswa <br/>
       $ exit <br/>
       kemudian gunakan opsi – sebagai berikut : <br/>
       $ su – mahasiswa <br/>
       $ exit <br/>
       Jelaskan perbedaan kedua utilitas tersebut. <p/>
       <img src="https://github.com/user-attachments/assets/203970c0-bed0-4108-aaca-e75d3119726f" width=500/>
       <br/>
       Penjelasan : <br/>
   <p> Perintah su mahasiswa hanya mengganti pengguna tanpa mengubah environment dan direktori kerja. Sedangkan su -          mahasiswa mengganti pengguna sekaligus menjalankan sesi shell login penuh untuk pengguna baru termasuk                 perpindahan ke direktori home pengguna.Perintah exit kemudian digunakan untuk keluar dari sesi shell pengguna          yang baru dan kembali ke pengguna sebelumnya. <p/>


## 2. Prompt String (PS)
  **a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan
       parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell** <br/>
       PS1='> ' <br/>
       export PS1 <p/>
       <img src="https://github.com/user-attachments/assets/37b5838c-c7d1-4c6c-af21-d2e7910af245" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/65f024a1-340f-4213-a959-9fbe6229fb83" width=500/>
       <br/>
  **b. Eksperimen hasil PS1 :** <br/>
       $ PS1=“\! > “ <br/>
       69 > PS1=”\d > “ <br/>
       Mon Sep 23 > PS1=”\t > “ <br/>
       10:10:20 > PS1=”Saya=\u > “ <br/>
       Saya=mahasiswa > PS1=”\w >” <br/>
       ~ > PS1=\h >” <p/>
       <img src="https://github.com/user-attachments/assets/8f7e66c8-400d-448a-b09a-010942aaa47a" width=500/>
       <br/>


## 3. Logout
  **Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout** <br/>
       Echo “Terima kasih atas sesi yang diberikan” <br/>
       Sleep 5 <br/>
       clear <p/>
       <img src="https://github.com/user-attachments/assets/84c0a3f7-2d1c-4146-a068-0101a72cdf0a" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/9f095562-a038-40c0-9e01-9d64fd431387" width=500/>
       <br/>


## 4. Bash script
  **a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :** <br/>
       p1.sh <br/>
       #! /bin/bash <br/>
       echo “Program p1” <br/>
       ls –l <p/>
       <img src="https://github.com/user-attachments/assets/ac42d935-6f46-4020-aa2d-9188d28c797b" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/71570685-f8f4-4465-8703-caae3e70d78c" width=500/>
       <br/>
       p2.sh <br/>
       #! /bin/bash ,br/>
       echo “Program p2” <br/>
       who <p/>
       <img src="https://github.com/user-attachments/assets/5bc704fe-849e-4051-8d45-7d28482c2891" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/1962a8bc-374c-440f-874c-62afeb124a38" width=500/>
       <br/>
       p3.sh <br/>
       #! /bin/bash <br/>
       echo “Program p3” <br/>
       ps x <p/>
       <img src="https://github.com/user-attachments/assets/5160ea5c-3435-4e2c-ac19-98a0a01e5e43" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/95da6bd4-0dc4-4b6d-aa97-c305e780b770" width=500/>
       <br/>
  **b. Jalankan script tersebut sebagai berikut :** <br/>
       $ ./p1.sh ; ./p3.sh ; ./p2.sh <br/>
       $ ./p1.sh & <br/>
       $ ./p1.sh $ ./p2.sh & ./p3.sh & <br/>
       $ ( ./p1.sh ; ./p3.sh ) & <p/>
       <img src="https://github.com/user-attachments/assets/fe350e20-c986-40eb-96ef-59a5d3aa7d46" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/0b8af137-a89d-4480-a70c-949d07e00651" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/e55e8ba6-551b-43dc-9f9a-2f0dbe2e7cbf" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/1f1c6f1d-d822-4745-ad26-5514190e7d0e" width=500/>
       <br/>


## 5. Jobs
  **a. Buat shell-script yang melakukan loop dengan nama pwaktu.sh,setiap 10 detik, kemudian menyimpan tanggal dan           jam pada file hasil.** <br/>
       #!/bin/bash <br/>
       while [ true ] <br/>
       do <br/>
         date >> hasil <br/>
         sleep 10 <br/>
       done <p/>
       <img src="https://github.com/user-attachments/assets/9f41ff42-ab87-4eb1-b26d-8ca40221ff69" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/1e42d5dd-e01f-4b75-94b5-ec7ee445c37c" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/0ee958f7-a678-41d4-8947-f5aa708c32b5" width=500/>
       <br/>
  **b. Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut :**         <br/>
       $ jobs <br/>
       $ find / -print > files 2>/dev/null & <br/>
       $ jobs<p/>
       <img src="https://github.com/user-attachments/assets/fbd390fe-7b26-4260-848a-10f59b77381e" width=500/>
       <br/>
       
  **c. Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background**
       $ fg %1 <br/>
       $ bg <p/>
       <img src="https://github.com/user-attachments/assets/194da0f8-4820-44c1-840e-19e412bc3807" width=500/>
       <br/>
  **d. Stop program background dengan utilitas kill**
       $ ps x <br/>
       $ kill [Nomor PID] <p/>
       <img src="https://github.com/user-attachments/assets/8a950830-5b3c-4cfa-a8a0-f81e8616a303" width=500/>
       <br/>
       <img src="https://github.com/user-attachments/assets/20cc2f48-6a5e-4700-a47e-f094807af1a7" width=500/>
       <br/>


## 6. History
  **a. Ganti nilai HISTSIZE dari 1000 menjadi 20** <br/>
       $ HISTSIZE=20 <br/>
       $ h <p/>
       <img src="
  **b. Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan** <br/>
       $ !-5 <p/>
  **c. Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer** <br/>
       $ !! <p/>
  **d. Ulangi instruksi pada history bufer nomor 150** <br/>
       $ !150 <p/>
  **e. Ulangi instruksi dengan prefix “ls”** <br/>
       $ !ls <p/>



       
