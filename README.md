# 🌐 Praktikum — Parsing Data HTTP, JSON & XML

Praktikum ini membahas **pengiriman request HTTP** serta **analisis response API** dengan membandingkan **format data JSON dan XML**. Pengujian dilakukan menggunakan **Postman** dan **Browser DevTools (Network Panel)** untuk mengamati **status code, headers, response time, dan response size**. Praktikum ini bertujuan memahami perbedaan karakteristik JSON dan XML dalam Web Service.

**Topik:** Parsing Data HTTP, JSON & XML

---

## 🧑‍🎓 Informasi Mahasiswa

| Informasi          | Data                                                       |
|--------------------|------------------------------------------------------------|
| Mata Kuliah        | Web Service Engineering                                    |
| Dosen Pengampu     | Muhayat, M.IT                                              |
| Praktikum / Proyek | P2 – Parsing data XML & JSON                               |
| Nama Mahasiswa     | Husna Norgina                                              |
| NIM                | 230104040056                                               |
| Kelas              | TI23B                                                      |
| Repo GitHub        | https://github.com/husna-norgina/P2-WSE-230104040056       |
| Tanggal Praktikum  | 29-09-2025                                                 |

---

## 🎯 Tujuan Praktikum

1. Mengirim request HTTP dan membaca response (status, headers, body, time, size).
2. Mengidentifikasi perbedaan struktur data **JSON** dan **XML**.
3. Membandingkan **response time** dan **response size** JSON vs XML.
4. Menggunakan **Postman** dan **Browser DevTools** dalam pengujian Web Service.
5. Menganalisis format data yang paling efisien untuk aplikasi web dan mobile.

---

## 🛠 Tools & Environment

### **Tools yang Digunakan**

* Postman
* Browser (Chrome / Edge / Firefox)
* JSONPlaceholder API
* HTTPBin API
* GitHub (Repository Dokumentasi)

---

## 🌍 API yang Digunakan

### 🔹 JSONPlaceholder (JSON)

API publik untuk simulasi REST API berbasis JSON.

**Endpoint:**

```
https://jsonplaceholder.typicode.com/posts/1
```

### 🔹 HTTPBin (XML)

API publik untuk pengujian response berbasis XML.

**Endpoint:**

```
https://httpbin.org/xml
```

---

## 🔁 Pengujian API

### 🔵 1. GET — Parsing Data JSON (Postman)

| Method | Endpoint   | Keterangan                      |
| ------ | ---------- | ------------------------------- |
| GET    | `/posts/1` | Mengambil data post format JSON |

**Hasil:**

![GET JSON](evidence/1.%20GET%20JSON.png)

Menampilkan satu objek JSON.
Server merespons status **200 OK**.

Response dianalisis berdasarkan **Time, Size, Headers, dan Body**.

---

### 🟡 2. GET — Parsing Data XML (Postman)

| Method | Endpoint | Keterangan                |
| ------ | -------- | ------------------------- |
| GET    | `/xml`   | Mengambil data format XML |

**Hasil:**

![GET XML](evidence/2.%20GET%20XML.png)

Menampilkan struktur XML berbasis tag.
Server merespons status **200 OK**.

Response time relatif lebih lambat dibanding JSON.

---

### 🔵 3. GET — Parsing Data JSON (Browser DevTools)

| Method | Endpoint   | Keterangan                               |
| ------ | ---------- | ---------------------------------------- |
| GET    | `/posts/1` | Analisis response JSON via Network Panel |

**Hasil:**

![Browser JSON](evidence/3.%20Browser%20JSON.png)

Data JSON ditampilkan di tab **Preview/Response**.

Informasi **Transferred Size** dan **Timing** dianalisis.

---

### 🔴 4. GET — Parsing Data XML (Browser DevTools)

| Method | Endpoint | Keterangan                     |
| ------ | -------- | ------------------------------ |
| GET    | `/xml`   | Analisis XML via Network Panel |

**Hasil:**

![Browser XML](evidence/4.%20Browser%20XML.png)

Struktur XML ditampilkan pada tab **Response**.

Response time dan size dibandingkan dengan JSON.

---

## 📊 Tabel Perbandingan JSON vs XML

| Jenis Data | Tools    | Method | Status Code | Response Time | Response Size |
| ---------- | -------- | ------ | ----------- | ------------- | ------------- |
| JSON       | Postman  | GET    | 200 OK      | 47 ms         | 1.34 KB       |
| JSON       | DevTools | GET    | 200 OK      | 51 ms         | 1.0 KB        |
| XML        | Postman  | GET    | 200 OK      | 1.73 s        | 751 B         |
| XML        | DevTools | GET    | 200 OK      | 1.17 s        | 0.7 KB        |

---

## 📄 Laporan Praktikum 2

[230104040056_Husna Norgina_P2](<evidence/230104040056_Husna Norgina_P2.pdf>)


---

> Semua screenshot hasil uji endpoint dan laporan praktikum disimpan pada folder:  
> 📂 `./evidence/`

---

## 📊 Analisis Praktikum

* Format **JSON** memiliki struktur sederhana (key–value) sehingga parsing lebih cepat.
* Format **XML** menggunakan tag hierarkis yang membuat parsing lebih kompleks.
* Response time JSON jauh lebih cepat dibanding XML.
* DevTools cenderung menampilkan ukuran data aktual, sedangkan Postman menghitung payload total.
* JSON lebih efisien untuk aplikasi **web dan mobile modern**.
* XML masih relevan untuk **sistem enterprise** dan kebutuhan standar formal.

---

## ✅ Kesimpulan

Berdasarkan hasil praktikum, dapat disimpulkan bahwa **JSON lebih unggul dalam kecepatan dan efisiensi** dibandingkan XML. Hal ini menjadikan JSON format yang paling umum digunakan pada REST API modern. Sementara itu, XML tetap memiliki peran penting pada sistem enterprise atau layanan berbasis standar seperti SOAP. Praktikum ini memberikan pemahaman yang kuat mengenai analisis response API dan pemilihan format data yang tepat dalam pengembangan Web Service.

---

## 📌 Catatan

* Semua pengujian dilakukan menggunakan Postman dan Browser DevTools.
* Endpoint yang digunakan bersifat publik dan hanya untuk simulasi.
* Data tidak disimpan secara permanen di server.

---

📝 *Disusun oleh Husna Norgina (230104040056) — Praktikum 2 Web Service Engineering*
