# Gradle Custom Task Project  

Proyek ini merupakan contoh sederhana penggunaan Gradle untuk membuat tugas khusus (custom task) dan mengelola dependensi pustaka.  

## Tujuan  
Proyek ini dirancang untuk:  
1. Membuat tugas Gradle yang menerima parameter melalui CLI dan mencetak pesan ucapan.  
2. Mengintegrasikan pustaka pihak ketiga menggunakan sistem manajemen dependensi Gradle.  

## Fitur  
- **Custom Task**:  
  Tugas Gradle `greetingTask` mencetak pesan ucapan ke terminal dengan parameter nama yang dapat diberikan melalui CLI. Jika tidak ada parameter, nama default digunakan.  
  - Perintah untuk menjalankan:  
    ```bash
    ./gradlew greetingTask -Pnama=YourName
    ```
  - Contoh output:  
    ```
    Hello, YourName! Welcome to Gradle World!
    ```
  - Tanpa parameter:  
    ```
    Hello, Gradle User! Welcome to Gradle World!
    ```

- **Dependensi yang Ditambahkan**:  
  - **Guava** (versi 29.0-jre): Untuk utilitas koleksi dan alat tambahan.  
  - **JUnit** (versi 4.13): Untuk pengujian unit.
