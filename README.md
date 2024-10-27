 Flowchart dan kode python untuk menentukan bilangan terbesar dari 3 buah bilangan yang di inputkan
flowchart : 



![foto flowchart](https://github.com/user-attachments/assets/a7b05ca0-9d9b-4719-8910-081cc03664e8)
 
  penjelasan flowchart: 
1.	Mulai: 
    •	 Titik awal dari proses. Flowchart dimulai di sini. 
2.	Input A, B, C: 
    •	Pengguna diminta untuk memasukkan tiga bilangan: A, B, dan C. Ini adalah data yang akan dianalisis untuk menentukan bilangan terbesar. 
3.	A > B?: 
    •	Di sini, kita membandingkan bilangan A dan B. 
    •	Jika Ya, berarti A lebih besar dari B, dan kita akan membandingkan A dengan C. 
    •	Jika Tidak, maka kita lanjut ke langkah berikutnya untuk membandingkan B dengan C. 
4.	A > C?: 
    •	Jika A lebih besar dari B, kita membandingkan A dengan C. 
    •	Jika Ya, maka A adalah bilangan terbesar. 
    •	Jika Tidak, berarti C lebih besar atau sama dengan A, sehingga C adalah bilangan terbesar. 
    •	Setelah itu, kita akan menampilkan hasil. 
5.	B > C?: 
   •	Jika A tidak lebih besar dari B, kita membandingkan B dengan C. 
   •	Jika Ya, maka B adalah bilangan terbesar. 
   •	Jika Tidak, maka C adalah bilangan terbesar. 
   •	Setelah itu, kita akan menampilkan hasil. 
6.	Tampilkan Hasil: 
   •	Di langkah ini, hasil yang menunjukkan bilangan terbesar dari A, B, atau C ditampilkan kepada pengguna. 
7.	Selesai: 
  •	Proses berakhir di sini. Flowchart telah menyelesaikan tugasnya untuk menentukan bilangan terbesar.

kode python : 
        
            # Menentukan bilangan terbesar
        if bilangan1 >= bilangan2 and bilangan1 >= bilangan3:
            terbesar = bilangan1
        elif bilangan2 >= bilangan1 and bilangan2 >= bilangan3:
            terbesar = bilangan2
        else:
            terbesar = bilangan3
        
        # Menampilkan hasil
        print("Bilangan terbesar adalah:", terbesar)

penjelasan kode: 
1. Definisi Fungsi terbesar_dari_3(a, b, c):  
   - Fungsi ini menerima tiga parameter (a, b, dan c), yang merupakan bilangan yang diinput oleh pengguna.  
   - Fungsi memeriksa mana dari ketiga bilangan tersebut yang terbesar menggunakan pernyataan kondisional if, elif, dan else.  
2. Pernyataan if a >= b and a >= c: Memeriksa apakah bilangan a lebih besar atau sama dengan b dan c. Jika benar, fungsi mengembalikan nilai a sebagai bilangan terbesar.  
3. Pernyataan elif b >= a and b >= c: Jika kondisi pertama salah, pernyataan ini memeriksa apakah b lebih besar atau sama dengan a dan c. Jika benar, fungsi mengembalikan 
   nilai b sebagai bilangan terbesar.Pernyataan else: Jika kedua kondisi sebelumnya salah, ini berarti c adalah bilangan terbesar, sehingga fungsi mengembalikan nilai c.  
4. a = float(input("Masukkan bilangan pertama: ")): Menerima input dari pengguna untuk bilangan pertama dan mengonversinya menjadi tipe data float (bilangan desimal). Hal 
       yang sama dilakukan untuk bilangan kedua dan ketiga (b dan c).  
5. memanggil Fungsi terbesar_dari_3(a, b, c): Setelah ketiga bilangan dimasukkan, fungsi dipanggil untuk menentukan bilangan terbesar, dan hasilnya disimpan dalam variabel 
   hasil.  
6. Mencetak Hasil: Baris print(f"Bilangan terbesar adalah: {hasil}") mencetak bilangan terbesar yang dikembalikan oleh fungsi.      

Flowchart dan kode python untuk menentukan bilangan terbesar dari N bilangan yang diinputkan, untuk menentukan jumlah N, berikan masukan angka 0


![foto flowchart (2)](https://github.com/user-attachments/assets/65523f8f-aefd-4394-a0d0-ec7e9498599c)
  
  penjelasan flowchart : 
1.	Mulai : o Proses dimulai di sini. Ini adalah titik awal dari flowchart. 
2.	Inisialisasi : o max_number = -∞: Variabel max_number diinisialisasi dengan nilai terkecil (∞). Ini bertujuan agar angka pertama yang dimasukkan selalu lebih besar, 
   sehingga dapat diperbarui dengan benar. 
3.	Input Angka: o Program meminta pengguna untuk memasukkan angka. Pesan yang disampaikan adalah "Input angka (0 untuk selesai)". Jika pengguna memasukkan 0, proses akan 
   berhenti. 
4.	Cek Angka: o angka = 0?: Di sini, program memeriksa apakah angka yang dimasukkan adalah 0. 
     ▪	Jika Ya: Program akan melanjutkan ke langkah berikutnya, yaitu menampilkan max_number. 
     ▪	Jika Tidak: Program akan melanjutkan ke langkah untuk memperbarui jumlah N. 
5.	Update N: o N += 1: Jika angka bukan 0, maka jumlah N (jumlah angka yang dimasukkan) akan ditambah 1. Ini penting untuk melacak berapa banyak angka yang telah 
   dimasukkan. 
6.	Cek Bilangan Terbesar:  o angka > max_number?: Program memeriksa apakah angka yang baru dimasukkan lebih besar dari max_number. 
   ▪	Jika Ya: Jika angka baru lebih besar, maka nilai max_number diperbarui dengan angka tersebut. 
   ▪	Jika Tidak: Program tidak melakukan apa-apa dan kembali untuk meminta input angka berikutnya. 
7.	Kembali ke Input: o Setelah memeriksa dan mungkin memperbarui max_number, program kembali ke langkah input untuk meminta angka berikutnya dari pengguna. 
8.	Tampilkan max_number : o Setelah pengguna memasukkan 0, program menampilkan hasil akhir, yaitu max_number, yang merupakan angka terbesar dari semua angka yang telah 
   dimasukkan. 
9.	Selesai : o 	Menandakan akhir dari proses. Setelah hasil ditampilkan, program selesai.
   
kode python : 


         # Loop untuk input bilangan
        while True:
            bilangan = float(input("Masukkan bilangan (masukkan 0 untuk selesai): "))
            
        # Cek apakah pengguna menginput 0
        if bilangan == 0:
            break
        
        # Tentukan bilangan terbesar
        if terbesar is None or bilangan > terbesar:
            terbesar = bilangan
    
         if terbesar is not None:
             print("Bilangan terbesar adalah:", terbesar)
         else:
             print("Tidak ada bilangan yang dimasukkan.")

penjelasan kode python : 
1.	Definisi Fungsi terbesar_dari_N(): Fungsi ini tidak menerima parameter, tetapi terus meminta pengguna untuk memasukkan bilangan sampai 0 dimasukkan, dan pada akhirnya 
    mengembalikan bilangan terbesar yang ditemukan.  
2.	max_number = float('-inf'): Menginisialisasi variabel max_number dengan nilai negatif tak hingga (-∞). Ini memastikan bahwa bilangan apa pun yang diinput pengguna akan 
    lebih besar dari max_number pada awalnya.  
3.	Perulangan while True:  
    - Menggunakan loop while yang berjalan tanpa batas sampai terjadi peristiwa penghentian (yaitu, ketika break dipanggil).
    - Pada setiap iterasi, program meminta pengguna untuk memasukkan bilangan.  
4.	n = float(input("Masukkan bilangan (0 untuk berhenti): ")): Meminta pengguna untuk memasukkan sebuah bilangan dan mengonversinya menjadi tipe float. Pengguna akan terus 
    memasukkan bilangan sampai dia memasukkan 0.  
5.	Pernyataan if n == 0: break: Jika pengguna memasukkan 0, pernyataan if ini akan menghentikan loop dengan break. Ini artinya proses input bilangan akan berhenti.  
6.	Pernyataan if n > max_number: Jika bilangan yang baru dimasukkan (n) lebih besar dari max_number, maka max_number diperbarui dengan nilai n. Ini memastikan bahwa 
    variabel max_number selalu menyimpan bilangan terbesar yang diinput sejauh ini.  
7.	Mengembalikan Nilai max_number: Setelah loop berakhir (ketika 0 dimasukkan), program akan mengembalikan nilai max_number sebagai bilangan terbesar.  
8.	Memanggil Fungsi terbesar_dari_N(): Fungsi dipanggil, dan hasilnya (bilangan terbesar) disimpan di variabel hasil.  
9.	Mencetak Hasil: Baris print(f"Bilangan terbesar adalah: {hasil}") akan mencetak bilangan terbesar yang ditemukan dari input pengguna.

flowchart pada pertemuan ke 5 : 
![flowchart pertemuan ke 5](https://github.com/user-attachments/assets/25066987-0e3f-43cb-b4ad-ff05e0aa7ee7)

penjelasan flowchart : 
Mulai:
1. Langkah awal program. Menandakan bahwa proses akan dimulai.
   Inisialisasi max_value = 0: Di sini, variabel max_value diinisialisasi dengan nilai 0. Ini berfungsi sebagai tempat penyimpanan nilai maksimum yang akan ditemukan 
   selama input.
2. Input n dari pengguna:
   Program meminta pengguna untuk memasukkan angka. Nilai yang dimasukkan akan disimpan dalam variabel n.
   Apakah n = 0?:
3. Ini adalah langkah keputusan. Program memeriksa apakah nilai n yang dimasukkan adalah 0.
   Jika Ya: Program melanjutkan ke langkah 7 untuk mencetak nilai maksimum dan mengakhiri program.
   Jika Tidak: Program melanjutkan ke langkah 5.
4. Apakah n > max_value?:
   Program memeriksa apakah angka yang dimasukkan (n) lebih besar dari max_value saat ini.
   Jika Ya: max_value diperbarui dengan nilai n.
   Jika Tidak: Program tidak melakukan perubahan pada max_value.
   Kembali ke langkah 3:
5. Setelah memeriksa dan mungkin memperbarui max_value, program kembali ke langkah 3 untuk meminta input angka dari pengguna lagi.
   Cetak "Nilai maksimum adalah: max_value":
6. Setelah pengguna memasukkan 0, program mencetak nilai maksimum yang telah ditemukan selama proses input.
   Selesai:
7. Menandakan akhir dari program. Semua proses telah diselesaikan.

kode python : 

          max_value = 0
          
                   while True:
                   n = int(input("Enter a number(0 to stop):"))
             
               if n == 0:
                   break 
           
               if n > max_value:
                   max_value = n 
           
           print("The maximum value is:",max_value)

penjelasan kode : 
1. inisialisasi: max_value diinisialisasi dengan nilai 0.
2. Loop: Program memasuki loop tak hingga (while True).
3. Input Pengguna: Meminta pengguna untuk memasukkan angka.
4. Kondisi Berhenti: Jika pengguna memasukkan 0, loop akan berhenti.
5. Pembaruan Nilai Maksimum: Jika angka yang dimasukkan lebih besar dari max_value, maka max_value akan diperbarui.
6. Output: Setelah loop berakhir, program mencetak nilai maksimum yang ditemukan.


