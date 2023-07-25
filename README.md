# Chat App
Chat App adalah aplikasi web real-time chat yang dibangun dengan menggunakan teknologi React, MongoDB, Express, Node.js, dan Socket.IO. Aplikasi ini memungkinkan pengguna untuk berkomunikasi satu sama lain secara langsung melalui pesan teks.


## Demo
https://chat-app-2100016081.vercel.app/

## Panduan Penggunaan
Berikut adalah langkah-langkah untuk menggunakan Chat App:
#### Login/SignUp
Login atau signup menggunakan akun anda.
![](https://github.com/Wibiemahardhika22/chat-app-2100016081/blob/main/ss/ss1.png)
![](https://github.com/Wibiemahardhika22/chat-app-2100016081/blob/main/ss/ss2.png)
#### Cari User
Cari user yang ingin dichat dengan mengeklik icon `Cari User`. 
![](https://github.com/Wibiemahardhika22/chat-app-2100016081/blob/main/ss/ss3.png)
#### Mulai Chat
![](https://github.com/Wibiemahardhika22/chat-app-2100016081/blob/main/ss/ss4.png)
#### Membuat Grup
Pilih bagian `Grup Baru +` kemudian masukkan nama grup dan nama teman yang akan dimasukkan ke dalam grup tersebut.
![](https://github.com/Wibiemahardhika22/chat-app-2100016081/blob/main/ss/ss5.png)
#### Edit Grup
Klik icon mata pada sebelah kanan atas kemudian edit grup sesuai keinginan. (Grup hanya bisa diedit oleh admin/yang membuat grup).
![](https://github.com/Wibiemahardhika22/chat-app-2100016081/blob/main/ss/ss6.png)

## Panduan Instalasi

Berikut adalah langkah-langkah untuk menginstal dan menjalankan aplikasi Chat App di lingkungan lokal Anda:

#### 1. Clone Repositori
```bash
git clone https://github.com/Wibiemahardhika22/chat-app-2100016081.git
```
```bash
cd chat-app-2100016081
```
#### 2. Instal Dependensi
Backend
```bash
cd backend
npm install
```

Frontend
```bash
cd ..
cd frontend
npm install --legacy-peer-deps
```

#### 3. Konfigurasi File
Di dalam file `backend/.env`, atur variabel lingkungan berikut sesuai kebutuhan
```bash
PORT=
MONGO_URI=
JWT_SECRET=
```
#### 4. Update Link API
Pada bagian `frontend` di dalam file `Login, SignUp, GroupChatModal, MyChats, SideDrawer, SingleChat, UpdateGroupChatModal`, ganti link API menggunakan link API localhost anda. Contoh:
```bash
const { data } = await axios.post(
    "https://chat-app-2100016081-api.vercel.app/api/user/login",
    email, password },
    config
);

// Ubah menjadi
const { data } = await axios.post(
    "http://localhost:5000/api/user/login",
    email, password },
    config
);
```

#### 5. Menjalankan Aplikasi
Backend
```bash
cd backend
npm start
```

Frontend
```bash
cd frontend
npm start
```






## Authors

- [Wibie Mahardhika Adi - 2100016081](https://www.github.com/wibiemahardhika22)

