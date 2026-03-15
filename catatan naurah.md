# Matrix Inversion Lemma
## Definisi Matrix Inversion Lemma
    Matrix Inversion Lemma adalah rumus yang digunakan untuk menghitung invers dari matriks yang berbentuk penjumlahan matriks tanpa harus menghitung invers besar secara langsung. 
## Syarat Matrix Inversion Lemma 
    Agar rumus ini bisa digunakan: 
    Matriks A harus memiliki invers
    Matriks C harus memiliki invers 
    Dimensi matriks harus cocok untuk perkalian.
## Rumus
   **Keterangan**
1. $A$ (Matriks Utama)   
   Dimensi: $n \times n$.
   Syarat: Harus memiliki invers ($A^{-1}$) atau bersifat non-singular.
   Peran: Mewakili sistem awal atau basis data yang besar.
2. $C$ (Matriks Modifikasi)  
    Dimensi: $k \times k$.
    Syarat: Harus memiliki invers ($C^{-1}$).
    Peran: Mewakili inti dari perubahan yang ditambahkan ke sistem. Biasanya $k$ jauh lebih kecil dari $n$ ($k \ll n$).
3. $B$ (Matriks Penghubung Depan)  
    Dimensi: $n \times k$.
    Peran: Menyesuaikan dimensi dari ruang modifikasi ke ruang sistem utama.
4.  $D$ (Matriks Penghubung Belakang) 
    Dimensi: $k \times n$.
    Peran: Menyesuaikan dimensi kembali dari ruang sistem utama ke ruang modifikasi. 
