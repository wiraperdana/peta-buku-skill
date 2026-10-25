# Gaya visual peta buku

**Acuan visual tunggal:** buka [AI-Driven University](00_genai_framework_ai_driven_university.png) sebagai gambar sebelum mulai. Empat PNG lain dalam folder ini adalah arsip. Gunakan hanya jika pengguna secara eksplisit meminta acuan lain. Isi dan sitasi acuan tidak boleh disalin ke peta sumber baru.

## Geometri acuan

Koordinat berikut mengacu pada kanvas 960×540. Skalakan semua posisi, ketebalan garis, dan huruf secara seragam. Render final minimal 1920×1080; 2880×1620 lebih baik untuk teks kecil. Ikuti komposisi ini secara presisi, lalu ubah kata dan ikon sesuai sumber.

- Judul navy besar mulai sekitar `(18, 18)`, disusul satu baris subtitel. Subtitel harus berakhir sebelum tab baris atas.
- Panel konteks abu muda di kiri: `x=20–219, y=97–440`. Judul merah, tiga kotak ikon dengan satu di atas dan dua di bawah, garis pemisah, daftar ringkas, dan satu konsekuensi merah di bawah.
- Panah tebal navy mengarah dari panel kiri ke area utama pada `x=230–304, y≈234`. Label hubungan berada di bawah panah. Sampul sumber asli di `x=225–313, y=381–507`, dengan proporsi terjaga.
- Rel vertikal navy putus-putus membingkai area utama di `x≈318` dan `x≈922`, dari `y≈106` sampai `y≈433`.
- Pita hasil atas: bingkai `x=350–892, y=81–130`, tab navy `y=62–83`. Isi disekat tipis dan punya sitasi dekat klaim.
- Tiga kartu utama: `x=341–511`, `541–710`, `740–908`; `y=145–257`. Masing-masing memiliki ikon putih dalam lingkaran navy, judul, rujukan, garis tipis, dan penjelasan singkat tentang mekanismenya. Bila ada lebih dari tiga gagasan utama, pilih tiga yang menjawab pertanyaan pengguna atau buat seri peta. Jangan hanya menaruh nama program.
- Baris pendukung: bingkai `x=333–908, y=281–329`, tab navy di atasnya. Tempatkan komponen pendukung sumber dalam satu kelompok bernama dan bernomor bila sumber menyebut jumlahnya.
- Baris merah: bingkai `x=331–909, y=346–405`, tab merah di atasnya. Isi dengan prinsip atau kriteria lintas program yang benar-benar dinyatakan sumber. Sorot kartu pertama dengan garis merah.
- Empat kartu aksi navy: `y=413–446`, dengan panah kecil di antaranya. Pakai hanya untuk langkah yang dapat dipertanggungjawabkan sebagai urutan. Bila urutannya hasil sintesis, tandai sebagai sintesis. Jangan mengubah kegiatan paralel menjadi langkah berurutan.
- Pita kesimpulan navy: `x=451–910, y=454–502`. Satu kalimat yang merangkum hubungan utama. Footer sumber pada `y≈516`, dengan garis navy tipis memanjang ke kanan.

## Huruf, warna, dan ikon

- Cocokkan bentuk huruf acuan: judul memakai sans serif tebal yang lebar, seperti Arial Bold. Label dan isi kartu memakai sans serif padat, seperti Arial Narrow Bold dan Arial Narrow. Jangan memakai font dekoratif atau judul yang terlalu sempit.
- Gunakan navy tua `#00225d`, putih, panel abu `#f0f2f5`, garis biru muda, dan merah `#db111b`. Warna merah menandai satu lapisan penekanan, bukan dekorasi acak.
- Ikon utama: garis putih pada lingkaran navy. Ikon pada pita: garis navy pada bidang putih. Gambar ikon dan panah sebagai bentuk vektor atau raster terprogram agar tidak bergantung pada dukungan simbol font.
- Rujukan berada pada kartu yang memuat klaim. Pertahankan ukuran terbaca pada pratinjau 960×540; ringkas teks lebih dahulu sebelum mengecilkan huruf.

## Pemeriksaan sebelum kirim

1. Buka gambar acuan dan hasil secara berdampingan pada 960×540. Bandingkan setiap kotak, jarak, garis, sampul, ukuran huruf, dan pola ikon.
2. Ukur seluruh kotak teks. Pastikan teks dan ikon berada di dalam panel, tidak bersinggungan dengan garis atau tab, serta tidak muncul sebagai kotak kosong.
3. Periksa setiap kelompok bernomor terhadap sumber. Periksa nama, jumlah, hubungan, rujukan, dan arti panah. Tinjau hasil pada resolusi final dan 960×540.
4. Bila informasi penting tidak muat dalam pola acuan, bagi materi menjadi beberapa peta dengan pola visual yang sama.
