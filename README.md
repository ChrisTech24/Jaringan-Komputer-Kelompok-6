# Jaringan Komputer - Kelompok 6

Repository ini digunakan untuk dokumentasi Project Based Learning mata kuliah **Jaringan Komputer dan Komunikasi Data**.

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

Project ini membahas simulasi keamanan jaringan enterprise dengan melakukan segmentasi jaringan berdasarkan divisi perusahaan. Jaringan dibagi menjadi beberapa segmen, yaitu Admin IT, Guest, HRD, Keuangan, dan Server.

Pada tahap awal, project difokuskan pada perancangan topologi, IP plan, dan subnetting. Pada Progres 2, implementasi dilanjutkan ke pembuatan topologi di GNS3, konfigurasi segmentasi VLAN, serta routing antarsegmen menggunakan metode router-on-a-stick.

## Pembagian Segmen Jaringan

| Segmen | VLAN | Network/Prefix | Gateway |
|---|---:|---|---|
| Admin IT | 10 | 192.168.10.0/28 | 192.168.10.1 |
| Guest | 20 | 192.168.10.16/28 | 192.168.10.17 |
| HRD | 30 | 192.168.10.32/28 | 192.168.10.33 |
| Keuangan | 40 | 192.168.10.48/28 | 192.168.10.49 |
| Server | 50 | 192.168.10.64/28 | 192.168.10.65 |

## Struktur Repository

```text
JARINGAN-KOMPUTER-KELOMPOK-6/
│
├── GNS3/
│   └── Kelompok6_Enterprise_Security_P2.gns3project
│
├── Laporan/
│   └── LAPORAN PROGRES 1 KELOMPOK 6.pdf
│
└── README.md