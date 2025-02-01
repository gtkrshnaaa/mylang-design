# mylang-design

---

## Dokumentasi Bahasa Pemrograman

### 1. **Deklarasi Variabel**
   - **Keyword:** `let` (untuk variabel yang bisa diubah), `const` (untuk variabel yang tidak bisa diubah).
   - **Tipe Data:** `string`, `int`, `float`, dan array.
   - **Contoh:**
     ```customlang
     let name string = "Calestia"
     let age int = 14
     const pi float = 3.14
     ```

### 2. **Kontrol Alur**
   - **`if-else`**: Pengkondisian standar.
     ```customlang
     if (age >= 18) {
         print("Adult")
     } else if (age >= 13) {
         print("Teenager")
     } else {
         print("Child")
     }
     ```

   - **`switch-case`**: Untuk memeriksa kondisi tertentu.
     ```customlang
     switch (age) {
         case 18:
             print("You're exactly 18 years old.")
             break
         case 14:
             print("You're a teenager.")
             break
         default:
             print("Unknown age")
     }
     ```

### 3. **Fungsi**
   - **Keyword:** `function` untuk mendeklarasikan fungsi.
   - **Sintaks:** 
     ```customlang
     function greet(name string) string {
         return "Hello, " + name
     }

     function add(a int, b int) int {
         return a + b
     }
     ```
   - **Pemanggilan fungsi:**
     ```customlang
     print(greet(name))  // Output: "Hello, Calestia"
     println("Sum of 3 and 4 is: " + add(3, 4))
     ```

### 4. **Pengulangan (Loop)**
   - **`for` Loop Standar (Mirip Java):**
     ```customlang
     for (int i = 0; i < 5; i++) {
         print("Iteration $i")
     }
     ```

   - **Penggunaan `for` tanpa array (looping biasa):**
     ```customlang
     for (int i = 0; i < 10; i++) {
         print("Count: $i")
     }

     let count int = 0
     for (int i = 0; i < 10; i++) {
         count = count + 1
         if (count == 5) {
             break  // keluar dari loop saat count mencapai 5
         }
         print("Count: $count")
     }
     ```

### 5. **Array**
   - **Deklarasi Array:** Menggunakan tipe data array.
     ```customlang
     let names string[] = ["Alice", "Bob", "Calestia"]
     let numbers int[] = [1, 2, 3, 4, 5]
     ```
   - **Akses Array:** Menggunakan indeks untuk mengakses elemen.
     ```customlang
     print("First name: $names[0]")
     print("First number: $numbers[0]")
     ```

### 6. **Output**
   - **`print`** dan **`println`** sekarang menggunakan gaya yang seragam:
     - **`print`**: Untuk mencetak output dalam satu baris.
     - **`println`**: Untuk mencetak output dengan tambahan baris baru.
     
     **Contoh:**
     ```customlang
     print("My name is $name and I am $age years old.")
     println("My name is $name and I am $age years old.")
     ```

### 7. **Tipe Data**
   - **Tipe data yang tersedia:**
     - `string`: Tipe data untuk teks.
     - `int`: Tipe data untuk angka bulat.
     - `float`: Tipe data untuk angka pecahan.
     - `array[]`: Tipe data untuk menyimpan koleksi elemen.
   
   - **Contoh tipe data:**
     ```customlang
     let name string = "Alice"
     let age int = 25
     let height float = 5.9
     let numbers int[] = [1, 2, 3]
     ```

### 8. **Import Modul**
   - Untuk mengimpor modul eksternal (jika ada).
     ```customlang
     import greet
     ```

### 9. **Export Modul**
   - **`export`** digunakan untuk mengekspor fungsi atau variabel agar bisa digunakan di modul lain.
   - **Contoh export:**
     ```customlang
     export function greet(name string) string {
         return "Hello, " + name
     }
     
     export let pi float = 3.14
     ```

### 10. **Sintaks Ekspresi**
   - **Penggabungan String dan Variabel**: Gunakan `$` untuk menggabungkan variabel dengan string.
     ```customlang
     print("My name is $name and I am $age years old.")
     ```

### 11. **Penggunaan `break` dalam Loop**
   - **`break`** digunakan untuk keluar dari loop lebih awal.
     ```customlang
     for (int i = 0; i < 10; i++) {
         if (i == 5) {
             break
         }
         print("Iteration $i")
     }
     ```

---

