# Dashboard SPI — BBGTK Provinsi Jawa Barat

Dashboard statis (satu file HTML, tanpa backend) untuk menampilkan hasil evaluasi mandiri dan verifikasi Satuan Pengawas Intern (SPI) BBGTK Provinsi Jawa Barat.

## Cara publish ke GitHub Pages

1. Buat repository baru di GitHub (public), misalnya `dashboard-spi-bbgtk-jabar`.
2. Upload file `index.html` dari folder ini ke root repository tersebut (bisa lewat web GitHub: **Add file → Upload files**, atau lewat `git push`).
3. Buka **Settings → Pages** di repository.
4. Pada **Source**, pilih branch `main` dan folder `/ (root)`, lalu klik **Save**.
5. Tunggu 1–2 menit, dashboard akan aktif di:
   `https://<username-github-anda>.github.io/<nama-repo>/`

## Update data

Data dashboard (nama unit, skor, temuan, rekomendasi, dll.) berada di dalam blok `<script>` menjelang akhir file `index.html`. Untuk memperbarui data periode berikutnya, cukup edit array/objek data di sana lalu upload ulang (atau commit) file yang sama.

## Struktur file

- `index.html` — seluruh dashboard (HTML + CSS + JS) dalam satu file, siap deploy langsung ke GitHub Pages tanpa proses build.
