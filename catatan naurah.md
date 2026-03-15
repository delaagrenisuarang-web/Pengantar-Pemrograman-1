# Matrix Inversion Lemma
## Definisi Matrix Inversion Lemma
    Matrix Inversion Lemma adalah rumus yang digunakan untuk menghitung invers dari matriks yang berbentuk penjumlahan matriks tanpa harus menghitung invers besar secara langsung. 
## Syarat Matrix Inversion Lemma 
    Agar rumus ini bisa digunakan: 
    Matriks A harus memiliki invers
    Matriks C harus memiliki invers 
    Dimensi matriks harus cocok untuk perkalian.
## Rumus
   # Matrix Inversion Lemma (Woodbury Identity)

**Matrix Inversion Lemma** adalah identitas aljabar linear yang sangat berguna untuk menghitung invers dari matriks yang mengalami perubahan kecil atau memiliki struktur tertentu tanpa harus menghitung ulang seluruh matriks dari nol.

---

## 1. Rumus Utama
Persamaan dasar untuk Matrix Inversion Lemma adalah:

$$[A + BCD]^{-1} = A^{-1} - A^{-1}B[C^{-1} + DA^{-1}B]^{-1}DA^{-1}$$

### Keterangan Simbol:
| Simbol | Deskripsi |
| :--- | :--- |
| **$A$** | Matriks utama berukuran $n \times n$ (harus memiliki invers/non-singular). |
| **$C$** | Matriks di tengah berukuran $k \times k$ (harus memiliki invers). |
| **$B$** | Matriks penghubung berukuran $n \times k$. |
| **$D$** | Matriks penghubung berukuran $k \times n$. |

---

## 2. Penjelasan Logika Pembuktian
Untuk membuktikan bahwa sisi kanan adalah invers dari sisi kiri, kita cukup mengalikan keduanya. Jika hasilnya adalah **Matriks Identitas ($I$)**, maka rumus tersebut terbukti benar.

### Langkah-langkah Pembuktian:

**Persamaan Pengujian:**
Kita kalikan rumus tersebut dengan $[A + BCD]$ dari sisi kanan (post-multiplying):
$$[A^{-1} - A^{-1}B(C^{-1} + DA^{-1}B)^{-1}DA^{-1}] \times [A + BCD]$$

**Langkah 1: Distribusi Suku Pertama ($A^{-1}$)**
$$A^{-1}(A + BCD) = I + A^{-1}BCD$$

**Langkah 2: Distribusi Suku Kedua**
Kita kalikan bagian panjang di belakang dengan $(A + BCD)$:
$$- A^{-1}B[C^{-1} + DA^{-1}B]^{-1}DA^{-1}(A + BCD)$$
$$= - A^{-1}B[C^{-1} + DA^{-1}B]^{-1}(D + DA^{-1}BCD)$$

**Langkah 3: Faktorisasi Cerdas**
Pada bagian $(D + DA^{-1}BCD)$, kita bisa mengeluarkan faktor $CD$ agar muncul bentuk $[C^{-1} + DA^{-1}B]$ yang sama dengan bagian inversnya:
$$= - A^{-1}B \underbrace{[C^{-1} + DA^{-1}B]^{-1} [C^{-1} + DA^{-1}B]}_{I} CD$$

**Langkah 4: Eliminasi**
Karena suatu matriks dikali inversnya menghasilkan $I$, maka bagian tengah "menghilang":
$$= - A^{-1}B(I)CD$$
$$= - A^{-1}BCD$$

**Langkah Akhir (Gabungan):**
$$= (I + A^{-1}BCD) - (A^{-1}BCD)$$
$$= I$$

> **Kesimpulan:** Karena hasil perkaliannya adalah Matriks Identitas ($I$), maka rumus **Matrix Inversion Lemma** terbukti valid.
