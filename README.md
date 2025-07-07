![1000030327](https://github.com/user-attachments/assets/aefd7f9c-a64f-4501-af8b-48898f997217)

Assalamualaikum warahmatullahi wa barakatuh.
Om Swastiastu, Namo Buddhaya, Salam Kebajikan.

## Tim pengerjaan 
Nama peserta: Dion Firmanda
Jurusan: D4 Teknik Komputer
Institusi: Politeknik Elektronika Negeri Surabaya-ITS

## Project website:
https://dion.firmanda.000webhostapp.com/
(Masih tahap pengerjaan)

# **Latihan Lab Pembuatan Kode menggunakan Model Kode Granite**
Gunakan Model IBM Granite untuk Pembuatan Kode dan Tugas Pemrograman

## Pendahuluan
Di lab ini, Anda akan menggunakan model IBM Granite untuk membuat kode Python untuk skenario tertentu. Anda akan menerapkan pengetahuan Anda tentang teknik prompting untuk menentukan dan menjalankan prompt untuk membuat kode menggunakan IBM Granite. 

## Persyaratan perangkat lunak 
Untuk menyelesaikan lab ini, Anda memerlukan akses ke akun Replicate, yang memungkinkan Anda menggunakan model AI untuk melakukan tugas. Anda juga memerlukan token API dari akun Replicate Anda. Token API seperti kunci digital yang memungkinkan lab terhubung dengan aman ke akun Replicate Anda. Token ini akan ditambahkan dengan aman ke lingkungan Google Colab Anda sehingga lab dapat berjalan dengan benar. Meskipun Anda tidak perlu tahu Python untuk mengikutinya, keakraban dengannya dapat membantu Anda lebih memahami kode yang dibuat selama lab. 

## Tujuan 
Setelah menyelesaikan lab ini, Anda seharusnya dapat: 

Menggunakan model IBM Granite untuk pembuatan kode dan tugas pemrograman.

 ## Langkah-langkah lab
Lab ini mengharuskan Anda untuk menyelesaikan langkah-langkah berikut:

- **Langkah 1: Buat akun GitHub**
- **Langkah 2: Buat akun Replicate**
- **Langkah 3: Daftar ke Google Colab**
- **Langkah 4: Muat notebook Jupyter dan inisialisasi model**
- **Langkah 5: Hasilkan kode menggunakan model IBM Granite**

## Perkiraan durasi penyelesaian
30 menit

## Hasil Program
![1000030252](https://github.com/user-attachments/assets/557b1eeb-97f9-4bdc-b3aa-e66e431ca5e2)
![1000030251](https://github.com/user-attachments/assets/84752d67-b741-4c51-876f-d3dd1840d8e5)

## Kesimpulan
Gambar ini memperlihatkan bagian lain dari notebook yang berbeda (sd_learn_cgo_lab1.ipynb) dibanding sebelumnya (lab2). Berikut analisisnya:

📄 Konten Teks dalam Gambar:

Ini adalah deskripsi singkat beberapa novel klasik, kemungkinan digunakan sebagai data mentah atau sumber informasi yang akan diproses atau ditampilkan di lab2. Isi ringkasannya:

1. The Great Gatsby

Penulis: F. Scott Fitzgerald

Tema: Kehidupan dekaden di era Roaring Twenties (Jay Gatsby dan Daisy Buchanan)



2. Pride and Prejudice

Penulis: Tidak disebutkan (tetapi diketahui: Jane Austen)

Tema: Romansa Mary dan Elizabeth Bennet di era Regency Inggris



3. The Hobbit

Penulis: J.R.R. Tolkien

Diterbitkan: 1937

Genre: Fantasi



4. The Lord of the Rings

Penulis: J.R.R. Tolkien

Genre: Fantasi epik



5. Animal Farm

Penulis: George Orwell

Diterbitkan: 1945

Genre: Satir politik terhadap Uni Soviet



6. Brave New World

Penulis: Aldous Huxley

Diterbitkan: 1932

Genre: Distopia fiksi ilmiah (deskripsi ini belum selesai di tangkapan layar)

🔗 Keterkaitan dengan Gambar Sebelumnya (lab2)

Gambar ini (lab1) kemungkinan merupakan:

Sumber data atau deskripsi teks yang dipakai untuk membuat tampilan daftar buku seperti di lab2.

Contoh pemrosesan data ke UI: dari teks deskriptif → menjadi kartu interaktif dengan judul, penulis, dan harga.

💡 Saran:

1. Minta bantuan untuk mengonversi data deskriptif ini jadi struktur JSON atau DataFrame.

2. Menambahkan fitur search, filter, atau urutkan di tampilan kartu.

3. Minta kode Python-nya untuk render buku sebagai kartu dengan Streamlit, Gradio, atau IPyWidgets.

5. Membuat kode Python-nya dan ubah teks ini jadi tabel atau JSON.


# **Latihan Lab 2: Mengoptimalkan Kode yang Dihasilkan AI Menggunakan Model IBM Granite**

## **Pendahuluan** 
Lab ini berfokus pada pengoptimalan kode yang dihasilkan AI menggunakan teknik perintah few-shot dengan model IBM Granite Code di Google Colab untuk mengoptimalkan kualitas pembuatan kode. Perintah few-shot memungkinkan model untuk mengambil dari beberapa contoh, sehingga memungkinkan keluaran yang lebih akurat dan bernuansa dibandingkan dengan pendekatan perintah zero-shot awal. 

Lab ini dibangun berdasarkan Lab 1, yang berfokus pada pembuatan kode menggunakan model Granite Code, dengan mengalihkan fokus untuk menyempurnakan keluaran model melalui teknik perintah few-shot. Latihan ini berfokus pada pengoptimalan komponen UI untuk membuat antarmuka yang lebih intuitif untuk toko buku daring, yang menunjukkan bagaimana menggabungkan contoh dapat meningkatkan kualitas dan ketepatan kode yang dihasilkan. 

Di lab ini, Anda akan menggunakan keluarga model IBM Granite Code yang dihosting di Replicate untuk mengoptimalkan kode Python yang menyempurnakan desain halaman arahan untuk toko buku daring.

 ## **Persyaratan perangkat lunak** 
Untuk menyelesaikan lab ini, Anda harus memiliki akses ke akun dengan Replicate untuk membuat panggilan inferensi model. Anda juga harus mendapatkan token API dari akun Replicate Anda, yang akan ditambahkan dengan aman sebagai rahasia Google Colab. Pemahaman terhadap Python tidaklah penting, tetapi dapat membantu untuk memahami kode yang dihasilkan. 

## Tujuan
Mengoptimalkan kode yang dihasilkan AI menggunakan model IBM Granite Code. 

## Langkah-Langkah Lab
Lab ini mengharuskan Anda untuk menyelesaikan langkah-langkah berikut: 
- Langkah 1: Buat **akun GitHub**.
- Langkah 2: Buat **akun Replicate**.
- Langkah 3: Daftar ke **Google Colab**.
- Langkah 4: Muat **Jupyter notebook** dan inisialisasi model.
- Langkah 5: Hasilkan kode menggunakan **few-shot prompt**.
- Langkah 6: **Optimalkan** kode yang dihasilkan AI.

## Perkiraan durasi untuk menyelesaikan 
30 menit

## Hasil Program 
![1000030271](https://github.com/user-attachments/assets/90e4b2e0-a4a3-4e12-8bbd-f3ac9caadddc)
![1000030270](https://github.com/user-attachments/assets/e0aa5211-f9dd-4747-8a27-8af6a8b4bc8e)
![1000030269](https://github.com/user-attachments/assets/5e7ca224-0d87-432d-9594-9a091bb4b9ee)


## Kesimpulan
Gambar ini adalah tangkapan layar dari antarmuka pengguna (kemungkinan dari Google Colab atau Jupyter Notebook di Google Colab, terlihat dari URL dan nama file .ipynb) yang menampilkan daftar buku dalam format kartu (card layout). Berikut adalah hasil analisisnya:

📋 Konten yang Ditampilkan:

Terdapat daftar buku, masing-masing dengan informasi berikut:

Judul Buku

Nama Penulis

Harga Buku


Contoh isi:

1. The Hobbit

Author: Author Name 3

Price: $30.00



2. The Lord of the Rings

Author: Author Name 4

Price: $40.00



3. Animal Farm

Author: Author Name 5

Price: $50.00



4. Brave New World (sebagian terlihat di bawah)

🧩 Komponen UI yang Terlihat:

Kartu (card) untuk setiap buku (desain modern, responsif).

Simbol filter di sebelah kiri atas (mungkin untuk menyaring daftar buku).

UI Google Colab:

Nama file: sd_learn_cgo_lab2.ipynb

Status RAM dan Disk di bagian atas.

Mode tampilan notebook (ada toolbar colab).

💡 Interpretasi Kemungkinan:

Ini adalah bagian dari proyek pembelajaran (lab atau demo) yang menampilkan data buku dalam format visual berbasis komponen frontend (kemungkinan menggunakan Gradio, Streamlit, atau IPyWidgets di Jupyter Notebook).

Bisa jadi ini adalah hasil rendering model atau data dari Python script/notebook.

Wassalamu'alaikum warahmatullahi wa barakatuh.
