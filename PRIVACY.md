# 🛡️ Kebijakan Privasi (Privacy Policy) — Latte_Cocoa Bot

*Terakhir Diperbarui: 25 Juli 2026*

Kebijakan Privasi ini menjelaskan bagaimana **Latte_Cocoa** (selanjutnya disebut "Bot", mencakup bot Latte dan Cocoa) mengumpulkan, menggunakan, menyimpan, dan melindungi informasi Anda. Dengan menambahkan Bot ke server Discord Anda, menggunakan perintahnya, atau masuk ke Web Dashboard kami, Anda menyetujui praktik data yang dijelaskan dalam kebijakan ini.

---

## 1. Informasi yang Kami Kumpulkan

Kami mengumpulkan data seminimal mungkin untuk memastikan fitur pemutaran musik, pengaturan kustom, integrasi Last.fm, dan Web Dashboard dapat berfungsi dengan baik.

### A. Data Otomatis dari Discord
Ketika Bot aktif di server Anda, kami membaca data berikut melalui API Discord:
*   **ID Pengguna & Nama Pengguna Discord:** Untuk mengidentifikasi siapa yang meminta lagu (*requester*), melacak kontributor lagu, mengelola playlist pribadi, dan memproses login dashboard.
*   **ID Server (Guild ID) & Nama Server:** Untuk menyimpan konfigurasi khusus server (seperti prefix kustom, volume default, dan peran DJ).
*   **ID Saluran Suara & Teks (Channel ID):** Untuk menghubungkan bot ke saluran suara yang tepat dan mengirim pesan pemutar musik di saluran teks yang sesuai.
*   **Status Suara (Voice State):** Untuk melacak keberadaan pengguna di saluran suara guna menerapkan pembatasan kendali musik (misalnya memastikan pengguna berada di saluran suara yang sama dengan bot).
*   **Role ID Pengguna:** Untuk memverifikasi kewenangan pengguna (seperti apakah mereka memiliki DJ Role atau izin administrator).

### B. Data yang Disimpan di Database Cloud (Turso/libSQL)
Kami menyimpan data berikut secara persisten di database cloud kami untuk mendukung fitur lanjutan bot:
*   **Pengaturan Server (Guild Settings):** Konfigurasi prefix, volume default, bahasa bot, DJ role yang ditentukan, status auto-play, pengaturan radio 24/7 (termasuk saluran dan mood radio), serta preferensi sticky embed.
*   **Cadangan Antrean (Queue Backup):** Data lagu dalam antrean saat ini yang dicadangkan agar pemutaran musik dapat dilanjutkan secara otomatis apabila bot terputus atau melakukan restart.
*   **Riwayat Pemutaran Lagu (Song History):** Catatan lagu yang telah diputar di server, meliputi judul lagu, nama artis, URL sumber, durasi lagu, ID dan nama peminta lagu, serta waktu lagu diputar.
*   **Pengaturan Pengguna (User Settings):** Volume personal, status suara, emoji kustom, prefix kustom, serta tautan akun Last.fm (nama pengguna Last.fm dan session key jika diaktifkan).
*   **Koleksi Playlist Pribadi (User Playlists):** Playlist kustom yang dibuat pengguna, nama playlist, status dibagikan (*shared*), daftar lagu di dalamnya (judul, artis, URL, sumber platform, gambar cover art, dan durasi).
*   **Lagu yang Disukai (Liked Songs):** Koleksi lagu yang ditandai sebagai favorit oleh pengguna (judul, artis, URL, durasi, dan cover art).

### C. Data Dashboard & API Web
Saat Anda masuk ke Web Dashboard menggunakan Discord OAuth2:
*   **Discord OAuth2 (Identify Scope):** Kami meminta izin akses minimal untuk membaca profil publik Anda (User ID, username, avatar, dan daftar server Anda) guna memverifikasi apakah Anda memiliki izin untuk mengontrol pemutar musik di server tertentu.
*   **Cookies & Sesi (Session Cookie):** Kami menyimpan cookie sesi di browser Anda yang berlaku selama 30 hari untuk menjaga status login Anda agar tidak perlu masuk ulang setiap kali membuka dashboard.

---

## 2. Bagaimana Kami Menggunakan Data Anda

Kami menggunakan data yang dikumpulkan semata-mata untuk mendukung fungsionalitas bot:
*   **Operasional Pemutaran Musik:** Menghubungkan bot ke saluran suara, memutar lagu yang diminta, dan menampilkan antarmuka Now Playing.
*   **Penyimpanan Preferensi:** Menyimpan pengaturan khusus server dan profil kustom Anda agar tetap konsisten setiap kali bot digunakan.
*   **Statistik & Rekomendasi:** Menghasilkan tangga lagu terpopuler (*Top Charts*), statistik pendengar, serta merekomendasikan lagu baru (menggunakan pencarian iTunes API berdasarkan artis favorit Anda).
*   **Integrasi Last.fm:** Mengirimkan data pemutaran lagu ke profil Last.fm Anda secara otomatis (*scrobbling*) jika Anda mengaktifkan fitur ini.
*   **Keamanan & Kontrol Dashboard:** Memastikan kontrol pemutaran di Web Dashboard hanya dapat diakses oleh pengguna yang berwenang (misalnya pengguna yang sedang berada di saluran suara yang sama dengan bot).

---

## 3. Pembagian Data dengan Pihak Ketiga

Kami **tidak pernah menjual, menyewakan, atau membagikan** data pribadi Anda kepada pihak ketiga untuk keperluan periklanan atau pemasaran. Data Anda hanya dikirimkan ke pihak ketiga berikut demi kebutuhan operasional bot:
*   **Discord API:** Seluruh interaksi bot tunduk pada [Kebijakan Privasi Discord](https://discord.com/privacy).
*   **Lavalink Nodes & Provider Audio (YouTube, Spotify, SoundCloud, dll.):** Kami mengirimkan informasi pencarian lagu atau URL lagu ke server Lavalink untuk memutar audio. Tidak ada data pribadi pengguna Discord yang dikirimkan ke layanan ini.
*   **Last.fm API:** Jika Anda mengintegrasikan akun Last.fm, data musik yang sedang diputar akan dikirim ke Last.fm sesuai dengan [Kebijakan Privasi Last.fm](https://www.last.fm/legal/privacy).
*   **iTunes API:** Digunakan secara anonim untuk mengambil rekomendasi lagu dan gambar cover album.

---

## 4. Retensi dan Penghapusan Data

Kami berkomitmen untuk tidak menyimpan data lebih lama dari yang diperlukan:
*   **Riwayat Pemutaran (History):** Riwayat pemutaran lagu (*Song History*) di server akan dihapus secara otomatis dari database setelah **30 hari**.
*   **Penghapusan Mandiri:** Anda dapat menghapus lagu dari playlist atau liked songs Anda kapan saja langsung melalui Web Dashboard atau perintah bot.
*   **Penghapusan Data Permanen:** Jika Anda ingin menghapus seluruh data pengguna Anda (termasuk playlist, liked songs, dan integrasi Last.fm) secara permanen dari database kami, Anda dapat menghubungi administrator bot.
*   **Data Server Setelah Bot Keluar:** Jika bot dikeluarkan dari server (*kick/leave*), data konfigurasi server akan tetap disimpan agar pengaturan Anda tidak hilang jika Anda mengundang bot kembali. Namun, pemilik server dapat meminta penghapusan data server secara permanen dengan menghubungi administrator bot.

---

## 5. Keamanan Data

Kami menerapkan langkah-langkah keamanan untuk melindungi data Anda:
*   Semua data disimpan pada **Turso Cloud Database** yang terlindungi dengan autentikasi token cloud yang ketat.
*   Transmisi data antara Bot, Web Dashboard, dan Discord API terenkripsi menggunakan protokol HTTPS/WSS aman.
*   Token API sensitif disimpan dalam file konfigurasi lingkungan (`.env`) yang terisolasi dari publik.

---

## 6. Perubahan pada Kebijakan Privasi ini

Kebijakan Privasi ini dapat diperbarui dari waktu ke waktu untuk menyesuaikan dengan fitur baru bot atau perubahan kebijakan Discord. Perubahan akan langsung berlaku setelah dokumen ini diperbarui di repositori bot. Penggunaan berkelanjutan atas layanan kami setelah perubahan kebijakan berarti Anda menerima kebijakan yang diperbarui tersebut.

---

## 7. Kontak dan Hubungi Kami

Jika Anda memiliki pertanyaan, keluhan, atau ingin mengajukan permohonan penghapusan data pribadi Anda, silakan hubungi tim pengembang/administrator bot melalui:
*   Mengirimkan pesan langsung ke pemilik bot (menggunakan ID yang tercantum dalam file konfigurasi bot).
*   Melalui server Discord resmi kami (jika tersedia).
