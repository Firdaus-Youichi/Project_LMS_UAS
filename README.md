Backend Simple LMS

Proyek ini adalah backend untuk aplikasi Learning Management System (LMS) sederhana yang dirancang sebagai studi kasus untuk pembelajaran pengembangan backend menggunakan Django dan Django Ninja.

---

Prasyarat

Pastikan Anda sudah menginstal Docker dan Docker Compose di sistem Anda.

---

🔧 Langkah-Langkah

Menjalankan Django
1. Kloning Repository

Mulailah dengan menyalin repository ini ke perangkat Anda:

git clone https://github.com/Firdaus-Youichi/Project_LMS_UAS.git
cd be_simple_lms

2. Buat dan aktifkan virtual environment di terminal vscode

python -m venv env
env\Scripts\activate 

3. Install Dependencies
Pastikan berada di folder yang ada file requirements.txt
pip install -r requirements.txt

4. Migrasi Database
python manage.py makemigrations
python manage.py migrate

5. Jalankan Server
python manage.py runserver

Menggunakan Docker

1. Kloning Repository

Mulailah dengan menyalin repository ini ke perangkat Anda:

git clone https://github.com/Firdaus-Youichi/Project_LMS_UAS.git
cd be_simple_lms


2. Membangun Aplikasi

Bangun dan jalankan container aplikasi menggunakan perintah berikut:

```bash
docker-compose up -d --build
```

3. Mengatur Database

Untuk mengatur struktur tabel di database, masuk ke shell container aplikasi `be_simple_lms` dan jalankan perintah berikut:

```bash
python manage.py makemigrations
python manage.py migrate
```

---

📚 Deskripsi

Proyek ini memanfaatkan framework Django sebagai backend utama, dilengkapi dengan Django Ninja untuk membangun API yang ringan dan efisien. Proyek ini bertujuan untuk memberikan pengalaman langsung dalam pengembangan backend menggunakan pendekatan containerized.

---

Nama: Firdaus Youichi Yamamoto
NIM: A11.2022.14607
