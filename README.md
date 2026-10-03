# 🌱 Smart Hydroponic Berbasis IoT

Proyek **Tugas Akhir** Pelatihan Berbasis Kompetensi (PBK) **UPT BLK Surabaya Gelombang 5** program **Embedded System (Mikrokontroler)**.

Sistem ini memantau kondisi air hidroponik secara real-time dan mengendalikan pemberian nutrisi serta penambahan air, baik secara manual melalui **panel tombol** maupun dari jarak jauh melalui **website**.

---

## 📌 Deskripsi Proyek

Smart Hydroponic adalah sistem hidroponik cerdas berbasis IoT yang membantu pembudidaya menjaga kualitas larutan nutrisi tanaman tanpa harus mengecek dan menakar secara manual terus-menerus. Data sensor ditampilkan pada dashboard website, termasuk ketinggian air sehingga volume air di bak penampung dapat diketahui kapan saja. Pengguna dapat mengontrol pompa langsung dari dashboard atau dari tombol fisik pada panel.

**Tanaman yang dibudidayakan:**
- 🥬 Pakcoy
- 🥬 Kangkung

---

## ✨ Fitur Utama

### 📊 Monitoring Real-Time
| Parameter | Keterangan |
|-----------|------------|
| 🌡️ Suhu Air | Memantau suhu larutan nutrisi |
| 🧪 pH Air | Memantau tingkat keasaman larutan |
| 💧 PPM Air | Memantau kepekatan nutrisi (TDS/PPM) |
| 📏 Ketinggian Air | Memantau jumlah air di bak penampung |

### 🎛️ Kontrol Aktuator
Tiga kontrol dapat dijalankan melalui **tombol pada panel** maupun **tombol pada website**:
1. **Tambah Nutrisi A**
2. **Tambah Nutrisi B**
3. **Tambah Air**

---

## 📁 Isi Repositori

| File | Deskripsi |
|------|-----------|
| `Bluprint Smart Hydroponic Berbasis IoT.pdf` | Dokumen blueprint: rancangan sistem, diagram blok, dan skema perancangan |
| `Hidroponik_RTOS_WM_2_1.ino` | Kode program Arduino (firmware mikrokontroler) |
| `index.html` | Halaman website dashboard monitoring dan kontrol |

---

## 🧰 Perangkat yang Digunakan

**Hardware**
- Mikrokontroler: `[contoh: ESP32]`
- Sensor suhu air: `[contoh: DS18B20]`
- Sensor pH: `[tipe sensor]`
- Sensor PPM/TDS: `[tipe sensor]`
- Sensor ketinggian air: `[contoh: ultrasonik / water level sensor]`
- Pompa/aktuator untuk Nutrisi A, Nutrisi B, dan air
- Relay/driver: `[tipe]`
- Panel tombol (3 tombol: Nutrisi A, Nutrisi B, Air)

**Software**
- Arduino IDE
- Library: `[daftar library yang digunakan]`
- HTML/CSS/JavaScript untuk dashboard website

---

## ⚙️ Cara Kerja Sistem

1. Sensor suhu, pH, PPM, dan ketinggian air membaca kondisi larutan di bak penampung.
2. Mikrokontroler mengolah data sensor dan mengirimkannya ke website melalui jaringan internet.
3. Website menampilkan data suhu, pH, PPM, dan ketinggian air secara real-time.
4. Pengguna dapat menekan tombol **Nutrisi A**, **Nutrisi B**, atau **Tambah Air** pada **panel** atau **website**.
5. Mikrokontroler mengaktifkan pompa yang sesuai untuk menambahkan nutrisi atau air ke bak penampung.

```
[Sensor Suhu / pH / PPM / Level Air] ──► [Mikrokontroler] ◄──► [Website Dashboard]
                                               │
                  ┌────────────────────────────┼────────────────────┐
           [Pompa Nutrisi A]           [Pompa Nutrisi B]       [Pompa Air]
                                               ▲
                                        [Panel Tombol]
```

---

## 🚀 Cara Menjalankan

1. **Clone repositori**
```bash
   git clone https://github.com/[username]/Pelatihan_Embedded_SmartHidroponic.git
```
2. **Upload program ke mikrokontroler**
   - Buka `Hidroponik_RTOS_WM_2_1.ino` di Arduino IDE.
   - Pasang library yang dibutuhkan, pilih board dan port yang sesuai.
   - Sesuaikan konfigurasi (WiFi/server) bila diperlukan, lalu upload.
3. **Buka dashboard**
   - Buka `index.html` di browser, atau hosting melalui GitHub Pages.
   - Pastikan perangkat dan website terhubung ke layanan/jaringan yang sama.

---

## 📷 Dokumentasi

> Tambahkan foto alat, tampilan dashboard, dan hasil tanaman pakcoy & kangkung di sini.
<img width="434" height="325" alt="Hasil_Projek" src="https://github.com/user-attachments/assets/a4e05d16-ac7a-4a86-ad9c-2264196f85f7" />

---

## 🎓 Informasi Pelatihan

- **Program**: Pelatihan Berbasis Kompetensi (PBK)
- **Penyelenggara**: UPT BLK Surabaya
- **Gelombang**: 5
- **Bidang**: Embedded System (Mikrokontroler)
- **Jenis Karya**: Tugas Akhir Pelatihan

---

## 👥 Pembuat

**Kelompok Smart Hidroponik**
Pelatihan Embedded System (Mikrokontroler) – UPT BLK Surabaya Gelombang 5

---

## 📄 Lisensi

Proyek ini dibuat untuk keperluan pembelajaran. `[Tambahkan lisensi, mis. MIT License, bila diinginkan]`
