# 💰 MoneyTrax - Personal Finance Tracker

MoneyTrax adalah aplikasi web sederhana untuk membantu pengguna mencatat pemasukan dan pengeluaran harian, serta memantau kondisi keuangan secara visual melalui grafik.

---

## 🚀 Tech Stack

- Laravel (Backend Framework)
- MySQL (Database)
- Blade Template Engine
- Chart.js (Data Visualization)
- Tailwind (UI Styling)

---

## ✨ Features

### 🔐 Authentication
- Register & Login user
- Logout system
- Protected dashboard per user

### 💰 Financial Management
- Tambah pemasukan (income)
- Tambah pengeluaran (expense)
- Edit & delete transaksi
- Kategori transaksi (makan, transport, dll)

### 📊 Dashboard
- Total saldo
- Total pemasukan
- Total pengeluaran
- Visualisasi grafik keuangan

### 📜 Transaction History
- Daftar semua transaksi
- Filter berdasarkan kategori / tanggal

---

## 🧱 Database Structure

### Users
- id
- name
- email
- password

### Categories
- id
- user_id
- name
- type (income / expense)

### Transactions
- id
- user_id
- category_id
- amount
- type
- description
- date

---

## ⚙️ Installation

```bash
git clone https://github.com/yourusername/moneytrax.git
cd moneytrax
composer install
npm install
cp .env.example .env
php artisan key:generate