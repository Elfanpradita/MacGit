# 🚀 Langkah Cepat SSH GitHub di macOS (✨ Sampai Langkah 4)

Ikuti langkah-langkah singkat ini buat nyambungin terminal macOS kamu ke GitHub via SSH! 🔐

---

## 🔑 1. Buat SSH Key

Buka Terminal dan jalankan:

```bash
ssh-keygen -t ed25519 -C "emailmu@gmail.com"
```

📝 Tekan **Enter** terus kalau nggak mau ubah lokasi atau pakai passphrase.

---

## 💻 2. Aktifkan SSH-Agent & Tambahkan Key

```bash
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
```

⚙️ Ini biar key kamu dikenali otomatis saat konek ke GitHub.

---

## 📋 3. Copy Public Key ke Clipboard

```bash
pbcopy < ~/.ssh/id_ed25519.pub
```

📎 Key kamu sekarang sudah siap ditempel ke GitHub!

---

## 🌐 4. Tambahkan ke GitHub

1. Buka [GitHub.com](https://github.com)
2. Klik foto profil kanan atas ➡️ **Settings**
3. Pilih **SSH and GPG keys**
4. Klik **New SSH Key**
5. Paste key dari clipboard 🔐
6. Klik **Add SSH Key**

🎉 Selesai! Lanjutkan ke langkah 5 buat ngetes koneksi.

---

> Butuh bantuan? DM aja 😎
