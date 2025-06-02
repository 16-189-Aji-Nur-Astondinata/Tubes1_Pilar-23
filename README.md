# TUGAS BESAR STRATEGI ALGORITMA 
## Kelompok Pilar 23
## Kelas RB

```bash
Anggota Kelompok:
Muhammad Naufal Fikri Akmal    123140132
Ausyaf Naufal Dinata           123140210
Aji Nur Astondinata            123140189
```
---

# Deskripsi Program

Diamonds adalah sebuah kompetisi pemrograman di mana setiap peserta diminta untuk membuat sebuah bot yang akan berhadapan dengan bot milik peserta lainnya. Tugas utama dari bot ini adalah mengumpulkan sebanyak mungkin diamond yang tersebar di arena permainan. Namun, proses pengumpulan diamond tidaklah mudah, karena terdapat berbagai rintangan yang dirancang untuk menambah tantangan dan keseruan dalam permainan. Untuk meraih kemenangan, peserta perlu merancang strategi yang cerdas dan menerapkannya dengan efektif pada bot mereka.

Program permainan Diamonds terdiri dari dua komponen utama:

1. Game engine, yang secara umum mencakup:

    - Kode backend permainan sebagai inti dari game ini, bertugas mengatur seluruh logika permainan serta menyediakan API untuk menghubungkan dengan tampilan 
      depan (frontend) dan bot pemain.

2. Bot starter pack, yang secara umum mencakup:

- Program pemanggil API yang digunakan untuk mengakses API dari backend.

- Program logika bot, yaitu bagian yang dikembangkan oleh kalian menggunakan algoritma greedy sebagai strategi untuk bot tim.

- Program utama (main) beserta berbagai utilitas pendukung lainnya yang dibutuhkan agar sistem dapat berjalan secara menyeluruh.

Repositori ini memuat implementasi strategi greedy berdasarkan nilai densitas tertinggi untuk pengembangan bot dalam permainan Diamonds. Strategi ini mengutamakan pengambilan diamond yang memiliki rasio poin terhadap jarak tempuh terbesar, sehingga bot dapat mengumpulkan poin secara lebih efisien.

## Komponen Permainan yang dibutuhkan

### 1. Game Engine yang harus di install adalah
- Node.js (https://nodejs.org/en)
- Docker Desktop (https://www.docker.com/products/docker-desktop/)

### 2. Bot Starter Pack Requirement yang harus di install
- Python (https://www.python.org/downloads/)


---

## Set Up Untuk Menjalankan Program
1. Game Engine yang harus di install:
   - Node.js (https://nodejs.org/en)
   - Docker Desktop (https://www.docker.com/products/docker-desktop/)
   - Yarn
     bash
     npm install --global yarn

2. Bot Starter pack yang harus di install:
   - Python (https://www.python.org/downloads/)

## Cara menjalankan program

1. **Jalankan game engine** dengan cara mengunduh starter pack game engine dalam bentuk file `.zip` yang terdapat pada tautan berikut:
   (https://github.com/haziqam/tubes1-IF2211-game-engine/releases/tag/v1.1.0)  
   Setelah melakukan instalasi, lakukan ekstraksi file `.zip` tersebut, lalu masuk ke root folder dari hasil ekstraksi file tersebut kemudian jalankan terminal.

   A. **Masuk ke direktori root dari game engine:**
   bash
   cd tubes1-IF2110-game-engine-1.1.0
   

   B. Instal dependencies menggunakan yarn:
   bash
   yarn
   
   C. Lakukan setup environment variable
   bash
   ./scripts/copy-env.bat
   

   D. Lakukan setup local database dengan membuka aplikasi docker desktop terlebih dahulu lalu jalankan perintah berikut di terminal
   bash
   docker compose up -d database
   

   E. Kemudian jalankan script berikut. Untuk Windows
   bash
   ./scripts/setup-db-prisma.bat
   
   F. Jalankan perintah berikut untuk melakukan build frontend dari game engine
   bash
   npm run build
   
   G. Jalankan perintah dibawah untuk memulai game engine
   bash
   npm run start
   

3. Jalankan bot starter pack dengan cara mengunduh kit dengan ekstensi .zip yang terdapat pada tautan berikut (https://github.com/haziqam/tubes1-IF2211-bot-starter-    pack/releases/tag/v1.0.1)

   A.  Lakukan ekstraksi file zip tersebut, kemudian masuk ke folder hasil ekstrak tersebut dan buka terminal b. Jalankan perintah berikut untuk masuk ke root directory           dari project

   B. Jalankan perintah berikut untuk masuk ke root directory dari project
   bash
   cd tubes1-IF2110-bot-starter-pack-1.0.1
   
   C. Jalankan perintah berikut untuk menginstall dependencies dengan menggunakan pip
   bash
   pip install -r requirements.txt
   
   D. Jalankan program dengan cara menjalankan perintah dibawah ini.
   bash
   python main.py --logic MyBot --email=your_email@example.com --name=your_name --password=your_password --team etimo
   
   E. Jika ingin hanya menjalankan satu bot saja atau beberapa bot dapat menggunakan .bat atau .sh script. Untuk windows
   bash
   ./run-bots.bat
   ```
   


---
