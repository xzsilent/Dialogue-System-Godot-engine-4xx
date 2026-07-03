# Dialog-System-Godot-engine-4xx

# Godot 3D Narrative Framework

Framework sistem dialog tingkat lanjut yang dirancang khusus untuk lingkungan **3D** menggunakan Godot Engine 4.x. Sistem ini berfokus pada penyampaian narasi yang imersif dengan transisi yang mulus antara *gameplay* 3D dan interaksi percakapan.

---

## Tentang Proyek
Framework ini dikembangkan untuk memberikan kontrol naratif penuh dalam game 3D. Sistem ini secara otomatis mengelola *input mode*, *camera state*, dan *pause logic* agar pemain dapat fokus sepenuhnya pada alur cerita tanpa terganggu oleh kendala teknis.

---

## Fitur Utama

*  **Sistem Dialog Dinamis:** Mendukung *typing effect* (per karakter) dengan kustomisasi BBCode untuk nama karakter, warna teks, dan *font* unik.
*  **Percabangan Cerita (Branching):** Sistem pilihan aksi yang fleksibel untuk menciptakan alur cerita yang mendalam dan responsif bagi pemain.
*  **Integrasi Input:** Peralihan otomatis antara *gameplay* 3D (Mouse Captured) dan *UI Mode* (Mouse Visible) yang mulus setiap kali dialog muncul.
*  **Performa Tinggi:** Menggunakan sistem *Signals* dan *Tweens* untuk memastikan transisi UI berjalan ringan dan sangat responsif di berbagai perangkat.
*  **Audio Feedback:** *Built-in* sistem suara untuk setiap ketikan dialog, memberikan efek "hidup" yang memuaskan dan terasa nyata.
*  **State Management:** Fitur *auto-pause* yang mengunci kontrol pemain selama dialog aktif untuk menjaga fokus narasi.

---

## Struktur Framework
Sistem ini dibangun dengan arsitektur **Node-Based** yang modular dan terisolasi:

*   **CanvasLayer:** Lapisan utama yang menjamin UI dialog selalu dirender di depan *viewport* 3D.
*   **Decoupled Signals:** Komunikasi menggunakan *Signals* (`percakapan_selesai`) untuk menjaga logika antar sistem tetap mandiri.
*   **Tween-Driven:** Penggunaan *Tween* untuk setiap animasi *fade-in/out*, memungkinkan perubahan visual yang halus secara *real-time*.

---

## Cara Penggunaan (Implementasi)
Sistem ini dirancang agar mudah diintegrasikan ke dalam proyek 3D apa pun:

1.  **Inisialisasi:** Panggil fungsi `Mulai_Percakapan()` dari script mana pun dengan mengirimkan `Array` berisi data dialog.
2.  **Format Data:** Gunakan struktur data sederhana dengan parameter `nama`, `warna`, `pesan`, dan `kecepatan` untuk kustomisasi per baris.

---

## Video:
https://youtu.be/WL1qp1FeYso?si=tdUoom0oK4ISPDKL



---

## Lisensi & Hak Cipta
**Proprietary License - All Rights Reserved.**
Seluruh kode sumber, desain UI, dan aset logika dalam repositori ini adalah milik pribadi. Dilarang mendistribusikan, menyalin, atau menggunakan kode ini untuk proyek apa pun tanpa izin tertulis dari pemilik hak cipta.
