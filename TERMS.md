# ⚖️ Ketentuan Layanan (Terms of Service) — Latte_Cocoa Bot

*Terakhir Diperbarui: 25 Juli 2026*

Selamat datang di **Latte_Cocoa** (selanjutnya disebut "Bot", mencakup bot Latte dan Cocoa). Dokumen Ketentuan Layanan ini mengatur penggunaan Anda atas Bot, perintah-perintahnya, serta antarmuka Web Dashboard kami.

Dengan menambahkan Bot ke server Anda, menggunakan perintahnya, atau masuk ke Web Dashboard kami, Anda setuju untuk terikat oleh Ketentuan Layanan ini. Jika Anda tidak menyetujui ketentuan ini, Anda tidak diperkenankan untuk menggunakan layanan kami.

---

## 1. Persyaratan Penggunaan

Dengan menggunakan Bot, Anda menyatakan bahwa:
*   Anda memiliki wewenang hukum untuk menyetujui ketentuan ini.
*   Anda akan menggunakan Bot sesuai dengan Ketentuan Layanan Discord (*Discord Terms of Service*) dan Pedoman Komunitas Discord (*Discord Community Guidelines*).
*   Anda tidak akan menggunakan Bot untuk aktivitas ilegal atau melanggar hukum setempat.

---

## 2. Aturan Penggunaan & Pembatasan

Untuk menjaga stabilitas sistem dan kenyamanan seluruh pengguna, Anda dilarang keras untuk:
*   **Menyalahgunakan Perintah (Spam):** Melakukan spam perintah secara berulang-ulang untuk membebani bot. Bot dilengkapi dengan sistem *Global Anti-Spam (Token Bucket)* yang membatasi pengiriman perintah (misalnya 3 perintah per 15 detik) dan pembatasan rate limit API Web Dashboard (100 request per menit). Tindakan bypass atau eksploitasi sistem ini akan berakibat pada pemblokiran akses.
*   **Eksploitasi Bug:** Memanfaatkan bug, celah keamanan, atau malfungsi bot untuk tujuan merusak atau mendapatkan keuntungan tidak sah. Jika Anda menemukan bug, Anda diharapkan untuk melaporkannya kepada administrator bot.
*   **Modifikasi atau Gangguan:** Mencoba merusak, mengganggu, atau memodifikasi server hosting bot, database Turso, node Lavalink, atau fungsionalitas Web Dashboard.

---

## 3. Hak Kekayaan Intelektual & Layanan Pihak Ketiga

*   **Konten Musik:** Bot ini memutar audio dengan melakukan pencarian dan streaming dari platform pihak ketiga (seperti YouTube, Spotify, SoundCloud, dan iTunes) melalui server Lavalink. Bot tidak menyimpan atau menghosting file musik tersebut di server kami.
*   **Tanggung Jawab Konten:** Anda bertanggung jawab penuh atas segala konten/lagu yang Anda minta untuk diputar melalui bot. Pastikan Anda tidak melanggar hak cipta atau ketentuan layanan dari platform penyedia audio tersebut. Kami tidak bertanggung jawab atas pelanggaran hak cipta yang disebabkan oleh lagu yang diminta oleh pengguna.
*   **Gambar Cover Art & UI:** Antarmuka visual (seperti *Frameless Now Playing Embed* dan *Image Rendering* berbasis Canvas) serta aset di dalam dashboard adalah hak kekayaan intelektual dari pengembang bot dan tunduk pada lisensi proyek ini.

---

## 4. Akses dan Kontrol Web Dashboard

Penggunaan Web Dashboard untuk mengontrol bot musik diatur oleh kebijakan hak akses internal bot:
*   **Kontrol Pemutaran:** Fitur kendali musik (seperti pause, resume, skip, volume, dan seek) di dashboard hanya dapat digunakan oleh pengguna yang berada di saluran suara (*Voice Channel*) yang sama dengan bot.
*   **Hak Istimewa (Otorisasi):** Pengguna dengan izin administrator server (`ManageGuild`), pengguna dengan *DJ Role* yang telah dikonfigurasi, pemanggil bot pertama (*Initiator*), dan pengguna yang diberi izin khusus oleh inisiator memiliki kontrol penuh atas pemutar musik. Pengguna lain tunduk pada sistem demokrasi voting untuk melakukan skip lagu.
*   **Keamanan Sesi:** Anda bertanggung jawab untuk menjaga keamanan akun Discord Anda. Segala tindakan yang dilakukan melalui akun Anda yang terhubung di Web Dashboard dianggap sebagai tindakan Anda sendiri.

---

## 5. Batasan Tanggung Jawab & Penafian (Disclaimer)

*   **Penyediaan "Apa Adanya":** Bot disediakan atas dasar "sebagaimana adanya" (*as is*) dan "sebagaimana tersedia" (*as available*). Kami tidak memberikan jaminan dalam bentuk apa pun bahwa bot akan selalu aktif 24/7 tanpa gangguan, bebas dari kesalahan, atau cocok untuk tujuan tertentu.
*   **Ketergantungan Pihak Ketiga:** Operasional bot sangat bergantung pada layanan pihak ketiga seperti Discord API, node Lavalink eksternal, dan API pencarian musik. Kami tidak bertanggung jawab atas kegagalan fungsi bot yang disebabkan oleh gangguan atau perubahan kebijakan pada layanan pihak ketiga tersebut.
*   **Batasan Kerugian:** Pengembang dan administrator Bot tidak bertanggung jawab atas kerugian tidak langsung, insidental, atau konsekuensial (termasuk kehilangan data server, kerusakan server Discord, atau gangguan komunikasi suara) yang timbul dari penggunaan atau ketidakmampuan menggunakan bot.

---

## 6. Pemblokiran dan Penghentian Layanan

Kami berhak untuk membatasi, menangguhkan, atau menghentikan akses Anda atau server Anda terhadap Bot dan Web Dashboard secara sepihak, tanpa pemberitahuan sebelumnya, apabila:
*   Anda atau server Anda terbukti melanggar Ketentuan Layanan ini.
*   Bot mendeteksi aktivitas mencurigakan atau penyalahgunaan sumber daya bot yang ekstrem dari server Anda.
*   Diminta oleh pihak berwajib atau kebijakan Discord.

---

## 7. Perubahan Ketentuan Layanan

Kami dapat merevisi Ketentuan Layanan ini sewaktu-waktu. Perubahan tersebut akan segera berlaku setelah dokumen yang diperbarui diunggah ke repositori atau diumumkan. Dengan terus menggunakan Bot setelah perubahan ketentuan, Anda menyatakan setuju untuk terikat oleh ketentuan baru tersebut.

---

## 8. Kontak & Hubungi Kami

Jika Anda memiliki pertanyaan tentang Ketentuan Layanan ini, silakan hubungi tim pengembang/administrator bot melalui pesan langsung ke pemilik bot (Owner IDs yang terdaftar pada konfigurasi `.env` bot).
