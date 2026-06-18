# Jaringan Komputer - Kelompok 6

Repository ini digunakan sebagai tempat dokumentasi dan pengumpulan Project Based Learning mata kuliah **Jaringan Komputer dan Komunikasi Data**.

## Judul Project

**Simulasi Keamanan Jaringan Enterprise**

## Anggota Kelompok

| NIM | Nama |
|---|---|
| 2401020160 | Muhammad Fauzi |
| 2401020151 | Christian Aprilio Sihite |
| 2401020157 | Andrian Yuza Swanda |
| 2401020165 | Adhie Mulia Sembiring |

## Deskripsi Project

Project ini membahas simulasi keamanan jaringan enterprise dengan tujuan membatasi akses antar divisi sesuai kebijakan keamanan. Jaringan dirancang dengan beberapa segmen, yaitu **Admin IT**, **Guest**, **HRD**, **Keuangan**, dan **Server**.

Implementasi project dilakukan secara bertahap sesuai progres yang ditentukan. Pada tahap awal, kelompok menyusun analisis kebutuhan, rancangan topologi, segmentasi jaringan, serta tabel IP dan subnetting. Setelah itu, implementasi dilanjutkan ke simulator GNS3 untuk melakukan routing, segmentasi jaringan, dan pengujian konektivitas dasar.

## Riwayat Dokumentasi Progres

Repository ini digunakan untuk menyimpan seluruh dokumen dan file pendukung project dalam satu tempat. Beberapa dokumen dapat berasal dari progres sebelumnya, kemudian diunggah ke repository sebagai arsip agar dokumentasi project lebih lengkap dan mudah diperiksa.

### Progres 1

Pada Progres 1, kelompok menyusun laporan perencanaan awal project. Isi Progres 1 meliputi:

- analisis kebutuhan jaringan,
- rancangan topologi,
- segmentasi jaringan,
- tabel IP dan subnetting,
- rencana routing,
- rencana implementasi ACL dan firewall.

Dokumen Progres 1 diunggah ke repository sebagai arsip dokumentasi tahap awal project.

### Progres 2

Pada Progres 2, kelompok mulai melakukan implementasi jaringan di GNS3. Fokus Progres 2 adalah **routing dan segmentasi jaringan**.

Implementasi yang dilakukan pada Progres 2 meliputi:

- pembuatan topologi di GNS3,
- penggunaan router Cisco 7200 sebagai router utama,
- penggunaan switch sebagai penghubung antar perangkat,
- pembagian VLAN berdasarkan segmen jaringan,
- konfigurasi IP address pada client/server,
- konfigurasi routing antarsegmen menggunakan metode router-on-a-stick,
- pengujian konektivitas dasar menggunakan ping.

File project GNS3 untuk Progres 2 telah ditambahkan pada folder `GNS3/`.

### Progres 3

Pada Progres 3, kelompok akan melanjutkan implementasi keamanan jaringan. Fokus Progres 3 adalah **ACL dan firewall**.

Rencana Progres 3 meliputi:

- penerapan ACL pada router,
- pembatasan akses jaringan Guest ke jaringan internal,
- pengujian akses yang diizinkan dan diblokir,
- dokumentasi hasil pengujian ping, traceroute, dan routing table,
- penyusunan screenshot konfigurasi dan video demonstrasi.

## Pembagian Segmen Jaringan

| Segmen | VLAN | Network/Prefix | Gateway | Contoh Host |
|---|---:|---|---|---|
| Admin IT | 10 | 192.168.10.0/28 | 192.168.10.1 | 192.168.10.2 |
| Guest | 20 | 192.168.10.16/28 | 192.168.10.17 | 192.168.10.18 |
| HRD | 30 | 192.168.10.32/28 | 192.168.10.33 | 192.168.10.34 |
| Keuangan | 40 | 192.168.10.48/28 | 192.168.10.49 | 192.168.10.50 |
| Server | 50 | 192.168.10.64/28 | 192.168.10.65 | 192.168.10.66 |

## Perangkat Simulasi

| Perangkat | Fungsi |
|---|---|
| Cisco 7200 | Router utama untuk routing antarsegmen |
| Ethernet Switch | Switch core untuk segmentasi VLAN |
| VPCS | Client/server simulasi untuk pengujian konektivitas |
| GNS3 | Simulator jaringan yang digunakan untuk implementasi project |

## Struktur Repository

```text
Jaringan-Komputer-Kelompok-6/
│
├── GNS3/
│   └── Kelompok6_Enterprise_Security_P2.gns3project
│
├── Laporan/
│   └── LAPORAN PROGRES 1 KELOMPOK 6.pdf
│
└── README.md