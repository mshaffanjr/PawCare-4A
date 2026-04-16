# 🐾 Software Requirements Specification (SRS)

## Paw Care Management System

---

## 1. **Introduction**

### 1.1 Purpose

Dokumen ini bertujuan untuk mendeskripsikan kebutuhan sistem **Paw Care**, yaitu aplikasi berbasis web untuk manajemen pet shop dan layanan perawatan hewan.

---

### 1.2 Scope

Paw Care digunakan untuk:

* Mengelola data produk dan stok
* Mencatat transaksi penjualan
* Mengelola layanan perawatan hewan (grooming)
* Menyimpan data pelanggan
* Menyediakan dashboard monitoring

---

### 1.3 Definitions

* **User**: Pengguna sistem (admin atau staff)
* **Produk**: Barang yang dijual (makanan, aksesoris, dll)
* **Transaksi**: Proses penjualan produk
* **Layanan**: Jasa perawatan hewan

---

## 2. **Overall Description**

### 2.1 Product Perspective

* Sistem berbasis web (fullstack)
* Frontend menggunakan Next.js
* Backend menggunakan Node.js + Express.js
* Database menggunakan PostgreSQL

---

### 2.2 User Characteristics

| User  | Deskripsi                     |
| ----- | ----------------------------- |
| Admin | Mengelola seluruh sistem      |
| Staff | Melakukan transaksi & layanan |

---

### 2.3 Operating Environment

* Browser modern (Chrome, Edge, Firefox)
* Node.js runtime
* Database PostgreSQL

---

### 2.4 Constraints

* Sistem membutuhkan koneksi internet
* Backend menggunakan REST API
* Database menggunakan relational model

---

### 2.5 Assumptions

* User memiliki akun login
* Data disimpan secara terpusat
* Sistem digunakan oleh pet shop skala kecil–menengah

---

## 3. **Functional Requirements**

### 3.1 Authentication

* FR-01: User dapat login
* FR-02: Sistem memvalidasi kredensial user

---

### 3.2 Product Management

* FR-03: User dapat menambah produk
* FR-04: User dapat mengedit produk
* FR-05: User dapat menghapus produk
* FR-06: Sistem menampilkan daftar produk

---

### 3.3 Inventory Management

* FR-07: Sistem menampilkan stok produk
* FR-08: Sistem mengupdate stok setelah transaksi

---

### 3.4 Transaction Management

* FR-09: User dapat membuat transaksi
* FR-10: Sistem menghitung total harga
* FR-11: Sistem menyimpan transaksi

---

### 3.5 Service Management

* FR-12: User dapat menambah layanan grooming
* FR-13: User dapat mengupdate status layanan

---

### 3.6 Customer Management

* FR-14: User dapat menyimpan data pelanggan
* FR-15: Sistem menampilkan riwayat pelanggan

---

### 3.7 Dashboard

* FR-16: Sistem menampilkan ringkasan data
* FR-17: Sistem menampilkan aktivitas terbaru

---

## 4. **Non-Functional Requirements**

### 4.1 Performance

* Sistem merespon request < 2 detik

### 4.2 Security

* Sistem menggunakan autentikasi login
* Password disimpan dalam bentuk terenkripsi

### 4.3 Usability

* Antarmuka mudah digunakan
* Navigasi jelas

### 4.4 Reliability

* Sistem berjalan stabil tanpa crash

### 4.5 Compatibility

* Sistem dapat diakses melalui browser desktop dan mobile

---

## 5. **System Architecture (Overview)**

* Frontend: Next.js
* Backend: Express.js
* Database: PostgreSQL + Prisma

---

## 6. **Future Enhancements**

* Pembayaran digital
* Notifikasi otomatis
* Role-based access control
* Mobile application
