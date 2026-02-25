# 📡 ZTE F670L – Default Firmware Collection

Koleksi **Firmware Default** untuk router **ZTE F670L** yang digunakan sebagai referensi pemulihan (recovery), downgrade, atau pengembalian ke kondisi bawaan pabrik.

> Repository ini dibuat untuk tujuan edukasi, backup, dan pemulihan perangkat sesuai kebutuhan teknis.

---

## 📌 Tentang Perangkat

**ZTE F670L** adalah perangkat GPON ONT (Optical Network Terminal) yang umum digunakan oleh berbagai ISP untuk layanan internet fiber. Router ini menggabungkan fungsi modem fiber dan WiFi router dalam satu perangkat.

---

## 🎯 Tujuan Repository

* 🔄 Restore ke firmware bawaan pabrik
* 🛠 Recovery router yang bootloop
* 🔍 Referensi teknis untuk analisis firmware
* 📦 Backup firmware sebelum modifikasi

---

## ⚙️ Cara Flashing (Gambaran Umum)

> ⚠️ Detail langkah dapat berbeda tergantung versi firmware & bootloader.

1. Login ke web admin router (biasanya `192.168.1.1`)
2. Masuk ke menu **Firmware Upgrade**
3. Upload file firmware `.bin` atau `.img`
4. Tunggu proses selesai (JANGAN matikan router)
5. Router akan restart otomatis

Alternatif metode:

* Via Telnet/SSH
* Via UART (untuk kondisi brick)
* Menggunakan tool ISP/maintenance khusus

---

## ⚠️ PERINGATAN PENTING

🚨 **MOHON BACA SEBELUM MELAKUKAN FLASHING**

Mengubah firmware router memiliki risiko serius, termasuk:

* ❌ Router menjadi **brick (mati total)**
* 🔒 Kehilangan akses ISP / konfigurasi GPON
* 📡 Tidak bisa terhubung ke OLT ISP
* 🧨 Kehilangan garansi perangkat
* 🔐 Serial number / LOID / credential GPON terhapus

### ❗ Jangan lakukan flashing jika:

* Anda belum pernah melakukan flashing firmware sebelumnya
* Tidak memahami risiko bootloop atau brick
* Tidak memiliki backup firmware asli
* Tidak memiliki akses recovery (UART / SPI programmer)
* Tidak memahami konfigurasi GPON (LOID / SN / Password)

Jika Anda tidak yakin dengan apa yang Anda lakukan, **JANGAN LANJUTKAN**.

---

## 🔐 Catatan Tentang ISP Lock

Beberapa unit ZTE F670L dikunci oleh ISP tertentu. Firmware default belum tentu bisa:

* Menghapus ISP lock
* Mengganti profil GPON
* Mengakses menu tersembunyi
* Mengubah SN/LOID

Setiap unit bisa memiliki:

* Versi hardware berbeda
* Bootloader berbeda
* Signature firmware berbeda

---

## 🧪 Risiko & Tanggung Jawab

Dengan menggunakan file dari repository ini, Anda menyetujui bahwa:

* Semua risiko ditanggung oleh pengguna
* Kontributor tidak bertanggung jawab atas kerusakan perangkat
* Tidak ada jaminan kompatibilitas
* Tidak ada jaminan keberhasilan flashing

Gunakan dengan bijak dan penuh tanggung jawab.

---

## 📋 Rekomendasi Sebelum Flashing

✔ Backup firmware lama
✔ Screenshot semua konfigurasi penting
✔ Catat SN & LOID GPON
✔ Gunakan UPS agar tidak mati listrik saat flashing
✔ Pastikan firmware sesuai dengan versi hardware

---

## 🤝 Kontribusi

Kontribusi sangat diterima:

* Upload firmware versi lain
* Tambahkan dokumentasi recovery
* Berikan catatan kompatibilitas
* Laporkan bug / pengalaman flashing

Silakan buat Pull Request atau Issue.

---

## 📜 Lisensi

Repository ini hanya menyediakan file firmware untuk tujuan backup & edukasi.
Hak cipta firmware tetap milik vendor terkait.

---

## ⭐ Penutup

Repository ini dibuat untuk membantu komunitas teknis dan pengguna yang membutuhkan firmware default untuk pemulihan perangkat.

⚠️ Sekali lagi: **Flashing firmware tanpa pemahaman yang cukup dapat menyebabkan router mati permanen.**

Gunakan dengan risiko Anda sendiri.

---
