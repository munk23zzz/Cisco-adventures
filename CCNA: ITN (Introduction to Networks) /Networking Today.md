# Module 1: Networking Today — Rangkuman

> Sumber: Cisco Networking Academy — *Introduction to Networks v7.0 (ITN)*, Module 1

## 1. Jaringan Memengaruhi Kehidupan Kita

Komunikasi lewat jaringan sudah jadi kebutuhan penting, hampir setara dengan air, makanan, dan tempat tinggal. Berkat jaringan, kita bisa terhubung dengan siapa pun, di mana pun, tanpa batas geografis (istilahnya *"world without boundaries"*).

## 2. Komponen Jaringan

**Host / End Device**
Setiap komputer yang terhubung ke jaringan disebut *host* atau *end device*. Ada dua peran utama:
- **Server** — menyediakan informasi/layanan ke perangkat lain (contoh: email server, web server, file server).
- **Client** — meminta/mengambil informasi dari server (contoh: browser mengambil halaman web).

**Peer-to-Peer (P2P)**
Satu perangkat bisa berperan sebagai client sekaligus server. Cocok untuk jaringan yang sangat kecil.

| Kelebihan | Kekurangan |
|---|---|
| Mudah dipasang | Tidak ada administrasi terpusat |
| Tidak rumit | Kurang aman |
| Murah | Tidak scalable (sulit berkembang) |
| Cocok untuk tugas sederhana (share file/printer) | Performa lebih lambat |

**Perangkat lain dalam jaringan:**
- **End device** — tempat data berasal atau tujuan akhir data (PC, laptop, printer, dll).
- **Intermediary device** — menghubungkan end device satu sama lain, contoh: switch, access point, router, firewall. Tugasnya meneruskan data, menjaga jalur komunikasi, dan memberi tahu jika ada gangguan.
- **Media jaringan** — jalur fisik/nirkabel tempat data mengalir: kabel tembaga (listrik), kabel fiber optik (cahaya), dan wireless (gelombang radio).

## 3. Representasi & Topologi Jaringan

Diagram jaringan (*topology diagram*) memakai simbol untuk menggambarkan perangkat. Istilah penting: **NIC** (kartu jaringan), **port fisik**, dan **interface** (sering dipakai bergantian dengan "port").

Ada dua jenis topologi:
- **Topologi Logis** — menunjukkan perangkat, port, dan skema pengalamatan (IP).
- **Topologi Fisik** — menunjukkan lokasi fisik perangkat dan jalur kabel yang sebenarnya.

## 4. Jenis-Jenis Jaringan

Berdasarkan ukuran:
- **Small Home Network** — menghubungkan beberapa komputer dengan internet.
- **SOHO (Small Office/Home Office)** — menghubungkan kantor kecil/rumah ke jaringan korporat.
- **Medium to Large Network** — banyak lokasi, ratusan-ribuan komputer terhubung.
- **World Wide Network** — jaringan skala dunia, contohnya internet.

**LAN vs WAN**

| LAN | WAN |
|---|---|
| Menghubungkan perangkat di area terbatas | Menghubungkan banyak LAN di area geografis luas |
| Dikelola satu organisasi/individu | Biasanya dikelola oleh penyedia layanan (ISP) |
| Bandwidth internal tinggi | Kecepatan antar-LAN cenderung lebih rendah |

**Internet** adalah kumpulan LAN dan WAN di seluruh dunia yang saling terhubung, tidak dimiliki satu pihak, tapi diatur oleh badan seperti **IETF**, **ICANN**, dan **IAB**.

**Intranet vs Extranet**
- **Intranet** — jaringan privat internal organisasi, hanya bisa diakses anggotanya.
- **Extranet** — memberi akses terbatas ke pihak luar (misalnya mitra bisnis) ke sebagian data organisasi.

## 5. Koneksi Internet

**Untuk rumah/kantor kecil:**
| Jenis Koneksi | Deskripsi |
|---|---|
| Cable | Bandwidth tinggi, selalu aktif, dari penyedia TV kabel |
| DSL | Bandwidth tinggi, selalu aktif, lewat jalur telepon |
| Cellular | Memakai jaringan seluler |
| Satellite | Solusi untuk daerah tanpa ISP (pedesaan) |
| Dial-up | Murah, tapi bandwidth sangat rendah |

**Untuk bisnis:** Dedicated Leased Line, Ethernet WAN, Business DSL, dan Satellite — biasanya butuh bandwidth lebih tinggi dan koneksi khusus (*dedicated*).

**Converged Network**
Dulu, telepon, video, dan data punya jaringan kabel & teknologi masing-masing. Sekarang, *converged network* menggabungkan data, suara (voice), dan video dalam satu infrastruktur jaringan yang sama.

## 6. Jaringan yang Andal (Reliable Network)

Empat karakteristik dasar arsitektur jaringan:

1. **Fault Tolerance** — jaringan tetap jalan meski ada bagian yang gagal, karena punya banyak jalur (redundansi). Ini didukung oleh *packet-switched network*, di mana data dipecah jadi paket dan tiap paket bisa lewat jalur berbeda (berbeda dengan *circuit-switched network* yang pakai jalur tetap).
2. **Scalability** — jaringan bisa berkembang (menambah user/aplikasi baru) tanpa mengganggu performa yang sudah ada.
3. **Quality of Service (QoS)** — mekanisme untuk memprioritaskan jenis traffic tertentu (misalnya suara/video) agar tetap lancar saat bandwidth terbatas.
4. **Security** — mencakup keamanan infrastruktur (fisik) dan keamanan informasi, dengan tiga tujuan utama:
   - **Confidentiality** — hanya penerima yang sah bisa membaca data.
   - **Integrity** — data tidak berubah/dirusak selama pengiriman.
   - **Availability** — data selalu bisa diakses tepat waktu oleh pengguna yang sah.

## 7. Tren Jaringan Terkini

- **BYOD (Bring Your Own Device)** — pengguna bebas memakai perangkat pribadi (laptop, tablet, smartphone) untuk mengakses jaringan kapan saja, di mana saja.
- **Online Collaboration** — kolaborasi lewat tools seperti Cisco WebEx.
- **Video Communication** — video call/conference jadi kebutuhan utama komunikasi jarak jauh.
- **Cloud Computing** — menyimpan file/menjalankan aplikasi lewat server di internet, didukung oleh data center. Ada 4 jenis cloud:
  - **Public Cloud** — terbuka untuk umum (bayar per pemakaian atau gratis).
  - **Private Cloud** — khusus untuk satu organisasi/entitas tertentu.
  - **Hybrid Cloud** — gabungan public & private.
  - **Custom Cloud** — dibuat khusus untuk kebutuhan industri tertentu (misal kesehatan, media).
- Tren lain: **Smart Home Technology**, **Powerline Networking** (internet lewat kabel listrik), dan **Wireless Broadband** (via WISP/teknologi seluler).

## 8. Keamanan Jaringan

**Ancaman Eksternal:**
Virus, worm, trojan horse, spyware/adware, zero-day attack, serangan denial of service, pencurian data & identitas.

**Ancaman Internal:**
Perangkat hilang/dicuri, kesalahan pemakaian oleh karyawan, hingga karyawan yang berniat jahat.

**Solusi Keamanan:**
- Untuk jaringan kecil: antivirus, antispyware, dan firewall.
- Untuk jaringan besar: dedicated firewall, **ACL** (Access Control List), **IPS** (Intrusion Prevention System), dan **VPN** (Virtual Private Network).

## 9. Profesi di Bidang IT

- **CCNA (Cisco Certified Network Associate)** — sertifikasi yang membuktikan pemahaman dasar teknologi jaringan, kini juga mencakup topik IP, keamanan, wireless, virtualisasi, otomasi, dan network programmability.
- Ada juga jalur sertifikasi **DevNet** (untuk skill software development) dan sertifikasi **Specialist** sesuai bidang minat/pekerjaan.
- Peluang kerja bisa dicari lewat netacad.com (menu Careers → Employment Opportunities / Talent Bridge).

## Poin-Poin Kunci (Ringkasan Singkat)

- Jaringan menghubungkan kita secara global lewat berbagai media (kabel, fiber, wireless).
- Ada 2 jenis infrastruktur jaringan utama: **LAN** dan **WAN**.
- Jaringan yang andal harus punya 4 sifat: **fault tolerance, scalability, QoS, dan security**.
- Tren seperti **BYOD, kolaborasi online, video, dan cloud computing** mengubah cara kita berinteraksi.
- Keamanan jaringan penting di semua skala, baik ancaman dari luar maupun dalam.
- Sertifikasi **CCNA** adalah langkah awal yang relevan untuk berkarier di bidang jaringan.

---

## Istilah Penting

| Istilah | Arti Singkat |
|---|---|
| Host / End Device | Perangkat yang jadi asal atau tujuan data |
| Server / Client | Penyedia layanan / peminta layanan |
| NIC | Kartu jaringan pada perangkat |
| LAN / WAN | Jaringan area lokal / jaringan area luas |
| Intranet / Extranet | Jaringan privat internal / akses terbatas untuk pihak luar |
| Packet-switched | Data dipecah jadi paket, tiap paket bisa lewat jalur berbeda |
| QoS | Mekanisme prioritas traffic agar layanan tetap lancar |
| BYOD | Kebijakan memakai perangkat pribadi untuk kerja |
| VPN, ACL, IPS | Teknologi keamanan jaringan |
| CCNA | Sertifikasi dasar Cisco di bidang jaringan |
