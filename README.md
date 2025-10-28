# ☕ Proyek OOP Java: Sistem Data Pegawai dan Divisi

Repositori ini berisi kode sumber untuk tugas mata kuliah **Pemrograman Berorientasi Objek (OOP)**. Proyek ini dibuat menggunakan **Java** di **Apache NetBeans IDE**.

Studi kasusnya adalah program konsol sederhana untuk manajemen data pegawai dan divisi, yang secara khusus mendemonstrasikan penerapan konsep **Inheritance (Pewarisan)** dan **Komposisi**.

## 🎯 Konsep OOP yang Diterapkan

Ini adalah fokus utama dari proyek:

# 1. Inheritance (Pewarisan)
Konsep ini digunakan untuk membuat spesialisasi dari kelas `Pegawai`.

* **`Pegawai.java` (Superclass / Kelas Induk)**
    * Berisi atribut dan method umum yang dimiliki semua pegawai (misalnya: `nama`, `noKTP`, `alamat`, `gajiPokok()`).

* **`PegawaiTetap.java` (Subclass / Kelas Anak)**
    * Mewarisi (extends) dari `Pegawai`.
    * Memiliki atribut tambahan (misalnya: `tunjangan`).
    * Mungkin meng-override method (misalnya: `hitungGaji()` yang menyertakan tunjangan).

* **`PegawaiKontrak.java` (Subclass / Kelas Anak)**
    * Mewarisi (extends) dari `Pegawai`.
    * Memiliki atribut tambahan (misalnya: `upahHarian`, `jumlahHari`).
    * Meng-override method `hitungGaji()` sesuai dengan perhitungan upah harian.

# 2. Komposisi (Composition)
Konsep ini digunakan untuk menunjukkan hubungan "memiliki" (has-a) antara `Divisi` dan `Pegawai`.

* **`Divisi.java`**
    * Kelas ini "memiliki" (`has-a`) satu atau lebih objek `Pegawai`.
    * Implementasinya menggunakan `ArrayList<Pegawai>` atau array `Pegawai[]` untuk menyimpan daftar pegawai yang termasuk dalam divisi tersebut.
    * Ini menunjukkan bahwa sebuah `Divisi` *terdiri dari* `Pegawai`.

# 🛠️ Teknologi yang Digunakan
* **Java** (misal: JDK 11 atau yang lebih baru)
* **Apache NetBeans IDE** (misal: NetBeans 12.0)

# 🚀 Cara Menjalankan Proyek

Ada dua cara utama untuk menjalankan proyek ini:

# 1. Menggunakan Apache NetBeans (Direkomendasikan)
Cara termudah, karena ini adalah proyek NetBeans:
1.  Unduh atau clone repositori ini.
2.  Buka Apache NetBeans IDE.
3.  Pilih `File` > `Open Project...`
4.  Arahkan ke folder repositori yang telah Anda unduh.
5.  NetBeans akan otomatis mendeteksi proyeknya.
6.  Klik kanan pada nama proyek di *Project Explorer* dan pilih `Run` (atau tekan F6).

# 2. Menggunakan Terminal (Command Line)
Jika Anda tidak memiliki NetBeans, Anda dapat meng-compile dan menjalankannya secara manual.

1.  Clone repositori:
    ```sh
    git clone [URL_REPOSITORI_ANDA]
    ```
2.  Masuk ke direktori `src` (source):
    ```sh
    cd nama-proyek/src
    ```
3.  Compile semua file `.java` (pastikan nama `Main.java` sesuai dengan file utama Anda):
    ```sh
    javac *.java
    ```
    *(Catatan: Jika Anda menggunakan package, misal `com.proyek`, Anda harus berada di folder `src` dan menjalankan `javac com/proyek/*.java`)*

4.  Jalankan kelas utama (Main):
    ```sh
    java Main
    ```
    *(Atau jika menggunakan package: `java com.proyek.Main`)*

## 🧑‍💻 Pembuat
* **[Nama Anda]** - `[NIM Anda]`
* Mata Kuliah: Pemrograman Berorientasi Objek
