 Flowchart dan kode python untuk menentukan bilangan terbesar dari 3 buah bilangan yang di inputkan






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
    
    # Menampilkan hasil
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





