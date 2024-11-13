                               LANGKAH-LANGKAH MEMBUAT JAVA FRAME LOGIN MENGGUNAKAN PERSISTENCE

1.	Pertama-tama, buat tabel baru di database yang sama dengan tabel sebelumnya. Dalam kasus saya, tabel sebelumnya adalah MATA_KULIAH dan saya akan membuat tabel baru yaitu Login.
   ![image](https://github.com/user-attachments/assets/5453cb9d-249c-4334-ab56-b43cab378eed)
    Kemudian isi tabel Login dengan akun yang akan digunakan sebagai akun login. Contohnya seperti ini:
  	![image](https://github.com/user-attachments/assets/8f10151e-f44a-4efd-95e7-fc9b9e5eb90c)

2.	Beralih pada Netbeans, buat ‘Entity Classes from Database’ baru. Lalu koneksikan dengan database dimana tabel Login tadi berada.
   ![image](https://github.com/user-attachments/assets/86d02813-4419-4d53-9654-20c07865405f)
    Pada tahap ini, pilih tabel Login lalu klik ‘Add All’. Kemudian klik Next.
  	
3.	Setelah itu, akan muncul popup dan langsung klik Next > Next > Finish.
4.	Setelah selesai, buat lagi class ‘JFrameForm’ baru lalu buat desain untuk tampilan Login nya. Berikut contoh desain saya.
   ![image](https://github.com/user-attachments/assets/c89cf8dc-7593-4a00-9caf-79772fa24a0a)
    Kemudian seperti biasa,  ganti nama variable pada textfield dan button nya. Lalu klik kanan pada button Login lalu pilih Events > Action > actionPerformed.
  	
5.	Nah, Pada tahap ini mulai untuk koding button nya. Tetapi sebelumnya, pastikan untuk menghubungkan class dengan database nya. Berikut ini contoh kodingannya.
   ![image](https://github.com/user-attachments/assets/a1dab5d9-19b7-48db-aae9-d6e9c515d363)

6.	Lanjut untuk koding button Login nya, berikut adalah kodingannya.
   ![image](https://github.com/user-attachments/assets/cbf24082-4920-4c4b-a159-0a419e569f31)
    Pada kodingan diatas, pastikan persistenceUnitName nya sesuai dengan yang ada pada class persistence.xml. Tutorialnya ada pada Repositories saya di Pertemuan12. 
    Saya menggunakan em.find untuk mengambil sampel dari tabel Login. Jika username dan password yang diinput sesuai dengan sampel, maka akan berhasil login. Jika sebaliknya, maka akan menampilkan pesan “Username atau Password Salah”. Lalu jika berhasil login, maka otomatis akan membuka desktop Mata_Kuliah pada pertemuan 12. 

7.	Kemudian saat di run hasilnya akan seperti ini.
    ![image](https://github.com/user-attachments/assets/a8e22d75-7ae6-4dbd-a89c-e575a9dfe65e)
  	Setelah muncul seperti ini, masukkan data yang ada pada tabel anda, lalu klik Login.

8.	Terakhir, akan langsung masuk ke tampilan Mata Kuliah seperti ini. Selamat Mencoba! 😉
    ![image](https://github.com/user-attachments/assets/023fc439-47cf-4f0e-b1b1-c6c87a963c57)

   
