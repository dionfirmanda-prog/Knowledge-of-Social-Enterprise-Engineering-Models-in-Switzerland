![1000030327](https://github.com/user-attachments/assets/aefd7f9c-a64f-4501-af8b-48898f997217)

Assalamualaikum warahmatullahi wa barakatuh.
Om Swastiastu, Namo Buddhaya, Salam Kebajikan.

## Tim pengerjaan
![1000030739](https://github.com/user-attachments/assets/379d8831-d403-400b-b452-65213ef64897)

Saya baru saja menyelesaikan pelatihan AI dari Hacktiv8 dan IBM SkillsBuild! Program ini benar-benar ngebuka wawasan saya tentang bagaimana AI bisa bantu proses coding, mulai dari code generation sampai optimasi. Lewat materi yang praktis dan pembimbingan langsung dari instruktur, saya jadi makin percaya diri buat masuk ke dunia kerja dengan skill yang relevan. Sekarang, saya resmi tersertifikasi dalam topik Code Generation & Optimization using IBM Granite. Buat teman-teman yang masih mahasiswa dan pengen upgrade skill sambil kuliah, saya sangat merekomendasikan program ini! Cek kelas terdekatnya daftar segera di my.hacktiv8.com/ibmskillsbuild #Hacktiv8 #IBMSkillsBuild #AIuntukSemua #MahasiswaSiapKerja #StudentDevelopmentInitiative #GenerativeAI

Twibbonize: https://www.twibbonize.com/p/LbDDy3pgNlr4rtk8#google_vignette

1. Nama peserta: Dion Firmanda
2. Jurusan: D4 Teknik Komputer
3. Institusi: Politeknik Elektronika Negeri Surabaya-ITS
4. CV Saya: [Dion Firmanda - Resume.pdf](https://github.com/user-attachments/files/21112236/Dion.Firmanda.-.Resume.pdf)


## Presentasi Kami

https://github.com/user-attachments/assets/0852fd8f-5336-4252-8e70-38aba3dd2bca

Swiss dikenal karena infrastruktur sosial dan ekonominya yang kuat, dan ekosistem wirausaha sosialnya mencerminkan kekuatan ini. Negara ini memadukan inovasi bisnis, tanggung jawab sosial, dan tata kelola yang terdesentralisasi, sehingga menghasilkan berbagai model Rekayasa Wirausaha Sosial (SEE).

## Laporan Kerja Capstone Project:
Judul: Knowledge of Social Enterprise Engineering Models in Switzerland

Tujuan Pembelajaran:
1. Memahami tentang arsitektur model Granite 3.0 dan aplikasi perusahaannya.
2. Mempelajari cara memanfaatkan Granite-3.0-2B-Instruct untuk tugas-tugas seperti ringkasan, pembuatan kode, dan Tanya Jawab.
3. Mengeksplorasi inovasi IBM dalam teknik pelatihan yang meningkatkan kinerja dan efisiensi Granite 3.0.
4. Memahami komitmen IBM terhadap transparansi sumber terbuka dan pengembangan AI yang bertanggung jawab.
5. Menemukan peran Granite 3.0 dalam memajukan solusi AI yang aman dan hemat biaya di seluruh industri.

Langkah 1: Setup (Install Required Libraries)

![1000030807](https://github.com/user-attachments/assets/41fbc449-862c-4c94-9992-3fb8fe36bf6a)
![1000030806](https://github.com/user-attachments/assets/4e2351bb-fa55-41be-806c-1ef2c6e554dd)

Berdasarkan gambar pertama dan kedua yang Saya unggah, berikut ini analisis program yang sedang Saya jalankan di Google Colab:

📌 Isi Program:

Install required libraries:
!pip install torch torchvision torchaudio
!pip install accelerate
!pip install git+https://github.com/...

🧩 Penjelasan Baris per Baris:

1. !pip install torch torchvision torchaudio

Menginstal PyTorch dan modul pendukung:

torch: library utama untuk machine learning dan deep learning.

torchvision: untuk mengelola dataset dan transformasi gambar.

torchaudio: untuk memproses data audio menggunakan PyTorch.




2. !pip install accelerate

Library dari Hugging Face untuk mempermudah eksekusi model secara efisien, mendukung CPU, GPU, dan multi-device training.



3. !pip install git+https://github.com/...

Baris ini belum terlihat lengkap, tetapi biasanya digunakan untuk menginstal library langsung dari repositori GitHub.

⚙️ Proses Instalasi:

Teks output menunjukkan:

Beberapa library seperti torch, torchvision, dsb. sudah terinstal sebelumnya (Requirement already satisfied).

Sedang mengunduh dependensi CUDA dari NVIDIA seperti:

nvidia-cuda-runtime

nvidia-cublas

nvidia-cudnn

nvidia-cufft

dan lainnya...



📦 Ini menandakan sistem sedang menyiapkan backend CUDA (untuk menjalankan PyTorch di GPU).

⚠️ Catatan Penting:

Proses ini bisa memakan waktu lama karena file CUDA cukup besar.

Google Colab biasanya sudah punya CUDA, tapi kadang tambahan versi/komponen diunduh ulang untuk kompatibilitas.

Jika koneksi lambat, proses Downloading... bisa tampak stuck.

✅ Rekomendasi Jika Proses Lama atau Gagal:

1. Pastikan runtime-nya menggunakan GPU:

Klik Runtime → Change runtime type → Pilih GPU.



2. Tambahkan flag untuk mempercepat:

Misalnya --no-cache-dir untuk menghindari simpanan lokal:

!pip install --no-cache-dir accelerate



3. Tunggu hingga seluruh dependensi selesai terunduh dan terpasang.

Langkah 2: Model and Tokenizer Initialization

![1000030809](https://github.com/user-attachments/assets/1bc15ced-7194-4755-9961-f5f36c813988)

Gambar ini menunjukkan bahwa model Granite 13B sedang dalam proses pengunduhan file berat di Google Colab. Berikut analisis lengkap program dan statusnya:

✅ Tujuan Program:

Menjalankan model bahasa besar dari Hugging Face (ibm-granite/granite-13b-instruct-v0-1) menggunakan pustaka transformers, untuk keperluan inferensi (menjawab, melengkapi teks, dsb).

🧠 Penjelasan Tahapan dan Kode:

🔹 Kode Python:

import torch
from transformers import AutoModelForCausalLM, AutoTokenizer

device = "cuda" if torch.cuda.is_available() else "cpu"

model_path = "ibm-granite/granite-13b-instruct-v0-1"

tokenizer = AutoTokenizer.from_pretrained(model_path)
model = AutoModelForCausalLM.from_pretrained(model_path)
model.eval()

🔍 Penjelasan:

1. Mengecek apakah GPU tersedia (cuda) untuk efisiensi.


2. Menentukan path model di Hugging Face.


3. Memuat tokenizer dari Hugging Face.


4. Memuat model besar (13B = 13 miliar parameter).


5. Menetapkan model ke mode evaluasi (eval()).

⏳ Status Saat Ini (Dari Output):

Fetching 2 files: 0% [model-00001-of-00002.safetensors, ...]
0.00 / 5.00 GB

Model menggunakan format safetensors dan dipecah menjadi beberapa bagian.

Total ukuran file: 5 GB lebih.

Saat ini: belum mulai diunduh (0%), mungkin karena koneksi lambat atau sedang menunggu izin/memori.

⚠️ Catatan Penting:

1. File Sangat Besar

Model Granite 13B adalah LLM besar → tidak ringan untuk Google Colab (bahkan GPU RAM bisa kurang).



2. Risiko Gagal di Colab Gratis

Model sebesar ini bisa gagal karena:

RAM GPU/CPU tidak cukup

Runtime terputus karena waktu terbatas

Koneksi lambat




3. Autentikasi Hugging Face

Model Granite 13B memerlukan autentikasi token (HF_TOKEN) jika repositori tidak publik sepenuhnya.

Jika muncul error seperti:

The secret HF_TOKEN does not exist

Maka Saya perlu login terlebih dahulu:

from huggingface_hub import login
login("your_hf_token")

✅ Rekomendasi:

Jika Ingin Lanjut:

Gunakan runtime GPU (Menu Runtime → Change Runtime Type → GPU).

Login ke Hugging Face terlebih dahulu jika diminta.

Gunakan opsi device_map="auto" agar transformers memilih lokasi yang optimal:

model = AutoModelForCausalLM.from_pretrained(model_path, device_map="auto")


Jika Ingin Ringan:

Ganti ke model lebih kecil, seperti:

tiiuae/falcon-rw-1b

EleutherAI/gpt-neo-125M

distilgpt2

🎯 Kesimpulan:

Program Saya berfungsi benar.

Proses belum berjalan karena sedang mengunduh file besar (5 GB).

Colab gratis kemungkinan tidak cukup kuat untuk model Granite 13B.

Disarankan mencoba model lebih kecil untuk eksplorasi awal.

Langkah 3: Input Format for Instruction-based Queries

![1000030810](https://github.com/user-attachments/assets/99e55af7-853b-4c36-acf8-fdf78fe0d7ad)

Gambar yang Saya tampilkan menunjukkan kelanjutan dari notebook Python sebelumnya yang kini sudah membentuk prompt percakapan (chat) dan sedang menyiapkan input untuk model bahasa. Berikut analisis detailnya:

✅ Tujuan Program:

Mempersiapkan input dalam format percakapan (chat) agar bisa dikirim ke model bahasa seperti granite-13b-instruct-v0-1 dari IBM, yang mendukung chat-style prompting.

🧠 Penjelasan Kode:

📌 Bagian 1 – Mendefinisikan Chat:

chat = [
    {"role": "user", "content": "pertanyaan kamu di sini"}
]

Ini membuat daftar percakapan (chat history).

Format "role": "user" digunakan untuk menandai siapa yang berbicara (bisa juga "assistant").

"content" adalah isi pesan, misalnya: "Apa itu machine learning?"


📌 Bagian 2 – Menggunakan Template Tokenizer:

chat = tokenizer.apply_chat_template(chat, return_tensors="pt")

apply_chat_template() adalah fungsi dari tokenizer modern (seperti yang mendukung model instruct/chat).

Ini akan mengonversi format percakapan di atas menjadi input teks yang disesuaikan dengan template (misalnya menambahkan token seperti <|user|>, <|assistant|>).

return_tensors="pt" mengembalikan hasil dalam format tensor PyTorch.

🔄 Alur Selanjutnya (Belum Terlihat di Gambar):

Biasanya setelah baris ini, Anda akan:

output = model.generate(chat, max_new_tokens=100)

Lalu hasilnya didekodekan:

tokenizer.decode(output[0], skip_special_tokens=True)

✅ Kesimpulan Analisis:

Elemen	Status	Penjelasan

Input chat	✅ Siap	Format JSON sudah sesuai untuk model chat (role + content).
Tokenisasi dengan template	✅ Benar	Menggunakan .apply_chat_template() — sesuai dengan tokenizer modern.
Penggunaan PyTorch	✅ Sesuai	Output dalam bentuk tensor (pt) yang cocok untuk model generate().

🎯 Saran:

Jika ingin menguji model setelah ini, Saya bisa lanjutkan dengan:

with torch.no_grad():
    output = model.generate(chat, max_new_tokens=100)
response = tokenizer.decode(output[0], skip_special_tokens=True)
print(response)

Langkah 4: Tokenize the Input

![1000030811](https://github.com/user-attachments/assets/86d1579b-d4ea-4d0c-93af-6da2f6f95541)

Langkah 5: Generate a Response

![1000030812](https://github.com/user-attachments/assets/8810752a-0481-4ca1-a881-3bab294fadc1)

Langkah 6: Decode and Print the Output

![1000030813](https://github.com/user-attachments/assets/9787b9ec-2129-4160-8c44-6695a8004b08)

![1000030814](https://github.com/user-attachments/assets/7b00fd2d-ff59-4bb4-83bd-a2fb6079cd6e)

Langkah 7: Text Summarization
![1000030815](https://github.com/user-attachments/assets/1002b684-33c6-4a17-8645-8e04166c9dd9)

![1000030816](https://github.com/user-attachments/assets/81105b33-94cf-483b-884b-ca85bc1b9e5a)

Langkah 8: Question Answering
![1000030817](https://github.com/user-attachments/assets/1ab9328c-ccfe-43ef-9f1c-011825571717)

![1000030818](https://github.com/user-attachments/assets/45619940-cc04-4e7a-909e-1912e040b946)

Langkah 9: Code-Related Tasks
![1000030819](https://github.com/user-attachments/assets/2bcb929e-df89-4f94-8c7c-a5be3b8e8cc6)

## Kesimpulan Capstone Project
Granite-3.0-BB-Instruct adalah model yang paling aman menurut grafik ini.

Model ini memberikan proteksi terbaik terhadap konten berbahaya, diskriminatif, atau eksplisit.

Mistral-7B-Instruct membutuhkan peningkatan keamanan karena cenderung membiarkan lebih banyak konten berisiko lolos.

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

## Referensi
1. https://www.analyticsvidhya.com/blog/2024/10/ibm-granite-3-0-model/
2. https://github.com/niit-ibm/lp1-cgo-lab1 
3. https://github.com/niit-ibm/lp1-cgo-lab2
4. https://rentonesia.com/

Terima kasih atas penilaiannya. Wassalamu'alaikum warahmatullahi wa barakatuh.
