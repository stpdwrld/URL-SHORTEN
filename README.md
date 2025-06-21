# 🔗 URL Shortener - Cloudflare Workers

URL Shortener ringan dan cepat yang berjalan di atas **Cloudflare Workers**.  
Mendukung custom alias, proteksi password, dan penyimpanan efisien menggunakan **KV namespace** bernama `links`.

---

## 🚀 Fitur

- ✂️ Buat shortlink dengan alias custom (contoh: `your.site/stupidworld`)
- 🔐 Opsi proteksi sandi (password)
- ⚡ Cepat dan tanpa database, cocok untuk kebutuhan pribadi atau publik
- ☁️ Penyimpanan di **Cloudflare KV**
- 🌍 Bisa digunakan sebagai self-hosted redirector, anti-expired

---

## 🛠️ Setup KV (Key-Value Storage)

Agar URL Shortener ini bekerja dengan baik, Anda perlu menyiapkan KV namespace bernama links.

1. Buat KV namespace baru:

Masuk ke dashboard **Cloudflare → Workers → KV → Create Namespace**

Nama: **links**



2. Binding KV ke Worker:

Buka Worker **Settings > KV Namespace Bindings**

Tambahkan binding baru:

Variable name: **LINKS**

KV namespace: pilih links yang telah Anda buat

## 📄 License

MIT License  
Copyright © 2025 **Stupid World**

Permission is granted to use, copy, modify, and distribute this software for any purpose,  
with or without fee, under the conditions that the original copyright  
notice and this permission notice are included in all copies.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND.
