# 📡 WebSocket Server with Node.js

Proyek ini adalah contoh sederhana **WebSocket server** menggunakan **Node.js** dan pustaka `ws`. Server akan menerima koneksi WebSocket dari client dan dapat mengirim serta menerima pesan.

---

## 📦 Fitur

- Menyediakan server HTTP di port `8080`
- Menerima koneksi WebSocket
- Mengirim pesan awal ke client: `"Hello from the server!"`
- Menampilkan pesan yang diterima dari client di console

---

## 🛠️ Teknologi

- Node.js (v18 atau lebih baru disarankan)
- [ws](https://github.com/websockets/ws) – WebSocket library untuk Node.js

---

## 📥 Instalasi

1. **Clone repository ini:**

```bash
git clone https://github.com/rosdiyanto/ws-nodejs.git
cd ws-nodejs
```

2. **Pasang dependensi:**

```bash
npm install
```

3. **Jalankan server:**

```bash
npm start
```

> Pastikan `server.js` berisi kode utama WebSocket server.

---

## 🧪 Pengujian

Kamu bisa menguji koneksi dengan:

- Menggunakan WebSocket client seperti:
  - [WebSocket King](https://websocketking.com/)
  - [Postman WebSocket](https://www.postman.com/)
  - Atau via browser console:
    ```js
    const ws = new WebSocket("ws://localhost:8080");
    ws.onmessage = (e) => console.log("Server:", e.data);
    ws.send("Hello server");
    ```

---

## 🗂 Struktur File

```
.
├── server.js      # Kode utama WebSocket server
├── package.json   # Konfigurasi proyek Node.js
└── README.md      # Dokumentasi ini
```

---

## 📝 Catatan

- Server ini listen di `http://localhost:8080`
- Setiap koneksi WebSocket akan langsung menerima pesan dari server
- Semua pesan yang dikirim oleh client akan dicetak ke console

---

## 📃 Lisensi

MIT License
