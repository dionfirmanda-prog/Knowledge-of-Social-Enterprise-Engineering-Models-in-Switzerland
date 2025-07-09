![1000031003](https://github.com/user-attachments/assets/b14748de-7f0b-4ce3-816b-8ffedf273750)


Assalamualaikum warahmatullahi wa barakatuh.

## Tim pengerjaan
![1000030739](https://github.com/user-attachments/assets/379d8831-d403-400b-b452-65213ef64897)

![1000031533](https://github.com/user-attachments/assets/f902293a-d6bd-427b-bba3-8767658d2b1c)

![1000031512](https://github.com/user-attachments/assets/e036e5c0-4a11-407d-8c15-93fd6be0412c)

![1000031678](https://github.com/user-attachments/assets/c6f24532-ae1d-415e-a177-d3791cc1ca2b)

Saya baru saja menyelesaikan pelatihan AI dari Hacktiv8 dan IBM SkillsBuild! Program ini benar-benar ngebuka wawasan saya tentang bagaimana AI bisa bantu proses coding, mulai dari code generation sampai optimasi. Lewat materi yang praktis dan pembimbingan langsung dari instruktur, saya jadi makin percaya diri buat masuk ke dunia kerja dengan skill yang relevan. Sekarang, saya resmi tersertifikasi dalam topik Code Generation & Optimization using IBM Granite. Buat teman-teman yang masih mahasiswa dan pengen upgrade skill sambil kuliah, saya sangat merekomendasikan program ini! Cek kelas terdekatnya daftar segera di my.hacktiv8.com/ibmskillsbuild #Hacktiv8 #IBMSkillsBuild #AIuntukSemua #MahasiswaSiapKerja #StudentDevelopmentInitiative #GenerativeAI

Tugas Pendahuluan 1: Membuat akun Twibbonize: https://www.twibbonize.com/p/LbDDy3pgNlr4rtk8#google_vignette

![1000031381](https://github.com/user-attachments/assets/85966c0f-b571-466c-9fe8-c4072f2689bc)

Tugas Pendahuluan 2: Membuat akun Credly: https://www.credly.com/users/dion-firmanda.6525f296

![1000031379](https://github.com/user-attachments/assets/30e275f4-997d-4ba4-8918-0c5581bcb10e)

Tugas Pendahuluan 3: Membuat akun IBM SkillsBuild: https://skills.yourlearning.ibm.com/

![1000031380](https://github.com/user-attachments/assets/1c4221ba-d5c3-4c79-9917-c032361f711b)

Tugas Pendahuluan 4: Membuat akun Replicate: https://replicate.com/

![1000031382](https://github.com/user-attachments/assets/679179cf-5c47-4c73-b5b3-1687a0534442)

Tugas Pendahuluan 5: Membuat akun Google Colab: https://colab.research.google.com/drive/1RiIBE2MR8vEe2cblyLumtB6p_X2X0OWG?authuser=0

![1000031383](https://github.com/user-attachments/assets/bfc9a4c4-a041-4f34-98c5-ce324637709f)

Tugas Pendahuluan 6: Membuat akun Github: https://github.com/dionfirmanda-prog/Knowledge-of-Social-Enterprise-Engineering-Models-in-Switzerland

![1000031387](https://github.com/user-attachments/assets/a3f031b0-a3c3-4649-8205-b7b0d159bd3a)

Tugas Pendahuluan 7: Membuat akun LinkedIn: https://www.linkedin.com/in/dion-firmanda-3b1861373?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app

![1000031606](https://github.com/user-attachments/assets/0b6e2561-2eca-4459-96a5-4a5ea6167daf)

## Slide Presentasi untuk Capstone Project

https://github.com/user-attachments/assets/6eddd337-16f8-4556-b43f-b6fb20e4ef8e

## Analisis Presentasi
Model Knowledge of Social Enterprise Engineering (KSEE) di Swiss dalam konteks ekonomi yang tumbuh untuk manajemen bencana merupakan pendekatan inovatif yang menggabungkan kewirausahaan sosial, rekayasa sistem, dan manajemen pengetahuan untuk mengatasi tantangan sosial, termasuk bencana alam dan krisis kemanusiaan. Swiss, sebagai negara maju dengan ekosistem inovasi yang kuat, telah menerapkan model ini untuk mendorong solusi berkelanjutan terhadap bencana dan krisis melalui kolaborasi lintas sektor.

## Kode Program Capstone Project
class Mahasiswa:
def __init__(self, nm, no_induk):
  self.nama = str(nm);
  self.nim = str(no_induk);

def getNama(self):
  return self.nama;

def getNim(self):
  return self.nim;

def setNama(self, nm):
  self.nama = nm;

def setNim(self, no_induk):
  self.nim = no_induk;

DftrMhs = {};
loop = True;

print("===================================");
print("=         Daftar Mahasiswa        =");
print("===================================");
print("= # MENU                          =");
print("= 1. Tambah Mahasiswa             =");
print("= 2. Hapus Mahasiswa              =");
print("= 3. Tampilkan Semua Mahasiswa    =");
print("= 4. Cari Mahasiswa               =");
print("= 5. Edit Nama Mahasiswa          =");
print("= 6. Edit Nim Mahasiswa           =");
print("= 7. Jumlah Total Mahasiswa       =");
print("= 0. Keluar                       =");
print("===================================");

while(loop):
print("\n\n");
 menu = int(input("Masukan menu : "));

if menu == 1:
  nama = str(input("Masukan nama : "));
  nim = str(input("Masukan nim : "));
  mhs = Mahasiswa(nama, nim);
  DftrMhs[nim] = mhs;
elif menu == 2:
  nim = str(input("Masukan nim : "));
  if(nim in DftrMhs):
   del DftrMhs[nim];
  else:
   print("Data tidak ditemukan!!!");
elif menu == 3:
  for i in DftrMhs:
   print("Nama :", DftrMhs[i].getNama());
   print("Nim :", DftrMhs[i].getNim());
elif menu == 4:
  nim = str(input("Masukan nim : "));
  if(nim in DftrMhs):
   print("Nama : ", DftrMhs[nim].getNama());
   print("Nim : ", DftrMhs[nim].getNim());
  else:
   print("Data tidak ditemukan!!!");
elif menu == 5:
  nim = str(input("Masukan nim : "));
  if(nim in DftrMhs):
   namaBaru = str(input("Masukan Nama Baru : "));
   DftrMhs[nim].setNama(namaBaru);
  else:
   print("Data tidak ditemukan!!!");
elif menu == 6:
  nim = str(input("Masukan nim : "));
  if(nim in DftrMhs):
   nimBaru = str(input("Masukan Nim Baru : "));
   DftrMhs[nim].setNim(nimBaru);
   mhs = DftrMhs[nim];
   DftrMhs[nimBaru] = mhs;
   del DftrMhs[nim];
  else:
   print("Data tidak ditemukan!!!");
elif menu == 7:
  print("Jumlah Mahasiswa : ", len(DftrMhs));
elif menu == 0:
  loop = False;
else:

  print("XXXX");
  
## Penjelasan tentang Capstone Project

![1000031731](https://github.com/user-attachments/assets/c651cbd7-99de-4b7a-adb6-5a5d59f1aa7a)

Proyek ini adalah aplikasi manajemen data mahasiswa sederhana berbasis teks, yang dikembangkan menggunakan bahasa pemrograman Python di lingkungan Jupyter Notebook.

📝 Fungsi Utama Aplikasi:

Aplikasi ini menyediakan menu interaktif untuk:

1. Menambah mahasiswa (input nama dan NIM)


2. Menghapus mahasiswa berdasarkan NIM


3. Menampilkan semua data mahasiswa


4. Mencari mahasiswa berdasarkan NIM


5. Mengedit nama mahasiswa


6. Mengedit NIM mahasiswa


7. Menampilkan total jumlah mahasiswa


8. Keluar dari aplikasi



🎯 Tujuan Proyek:

Melatih logika pemrograman dasar seperti:

1. Input/output

2. List dan struktur data

3. Perulangan (while)

4. Percabangan (if-else)


Proyek ini cocok untuk pemula sebagai latihan CRUD (Create, Read, Update, Delete) sederhana di Python.

## **Latihan Lab Pembuatan Kode menggunakan Model Kode Granite**
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

## Hasil Program Lab1
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

## Hasil Program Lab2
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

## Referensi
1. https://github.com/niit-ibm/lp1-cgo-lab1 
2. https://github.com/niit-ibm/lp1-cgo-lab2

Terima kasih atas penilaiannya. Wassalamu'alaikum warahmatullahi wa barakatuh.
