# Dice Roller App

## Deskripsi
Aplikasi Dice Roller adalah aplikasi sederhana berbasis Android menggunakan Jetpack Compose. Aplikasi ini memungkinkan pengguna untuk melempar dadu virtual 6 sisi dengan menekan sebuah tombol.

## Fitur Utama
- Menampilkan gambar dadu.
- Memungkinkan pengguna untuk melempar dadu dengan menekan tombol "Roll".
- Gambar dadu akan diperbarui sesuai dengan hasil lemparan yang dihasilkan secara acak.

## Kekurangan
- Belum ada animasi transisi dice ketika di roll

## Struktur Kode
### 1. **MainActivity.kt**
File utama yang berisi komposisi UI untuk aplikasi ini.

#### **`DiceRollerApp()` (Composable Function)**
- Fungsi preview yang menampilkan UI utama aplikasi.
- Memanggil `DiceWithButtonAndImage()` untuk menyusun tampilan.

#### **`DiceWithButtonAndImage()` (Composable Function)**
- **Variabel State:**
  - `result` digunakan untuk menyimpan hasil lemparan dadu.
  - `imageResource` menentukan gambar dadu berdasarkan nilai `result` menggunakan `when`.
  
- **Layout:**
  - `Column` digunakan untuk menyusun elemen secara vertikal dengan `Alignment.CenterHorizontally` dan `Arrangement.Center` untuk membuat tata letak berada di tengah layar.
  - `Image` menampilkan gambar dadu sesuai dengan hasil lemparan.
  - `Spacer` digunakan untuk memberi jarak antara gambar dadu dan tombol.
  - `Button` memungkinkan pengguna untuk melakukan lemparan dadu dengan mengubah nilai `result` ke angka acak antara 1 hingga 6.

## Cara Kerja
1. Saat aplikasi pertama kali dijalankan, dadu akan menampilkan angka 1 secara default.
2. Ketika tombol "Roll" ditekan, nilai `result` diperbarui dengan angka acak antara 1 hingga 6.
3. Gambar dadu berubah sesuai dengan angka yang dihasilkan.
4. Proses ini bisa diulang terus dengan menekan tombol "Roll".


## Cara Menjalankan Aplikasi
1. Buka proyek ini di Android Studio.
2. Jalankan aplikasi pada emulator atau perangkat fisik.
3. Tekan tombol "Roll" untuk melempar dadu dan melihat perubahan angka.

## Screenshot
![image](https://github.com/user-attachments/assets/84c8a822-060d-4aab-9bfc-1b7230a52911)


## Selamat Mencoba :))

