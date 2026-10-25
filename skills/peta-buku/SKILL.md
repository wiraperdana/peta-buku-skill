---
name: peta-buku
description: Membuat infografis landscape yang memetakan kerangka dan alur isi buku atau materi yang dilampirkan (PDF, PPT/PPTX, Markdown, DOCX, gambar, dan format lain yang dapat dibaca), dengan rujukan bagian sumber pada gambar. Dapat mengarahkan peta ke pertanyaan atau konteks penerapan tertentu, dengan sintesis yang dibedakan dari isi sumber. Pakai saat pengguna meminta peta buku, peta isi materi, atau infografis kerangka berpikir dari dokumen.
---

# Peta buku

Buat satu infografis 16:9 per sumber atau per cakupan yang diminta. Hasil harus menunjukkan hubungan antargagasan dan urutan logis materi, bukan hanya daftar bab. Pengguna dapat memberi arah penerapan, misalnya pelajaran reformasi arsitektur digital bagi AI Policy. Dalam mode itu, pisahkan isi sumber dari implikasi yang Anda simpulkan.

## Masukan dan pembacaan

1. Identifikasi semua lampiran, halaman web, atau path yang disebut. Baca materi secara langsung dengan alat yang sesuai format. PDF dan gambar berisi teks memerlukan pemeriksaan halaman visual atau OCR saat ekstraksi teks tidak lengkap. Untuk PPT/PPTX, pertahankan nomor slide. Untuk audio atau video, gunakan timestamp bila alat transkripsi tersedia. Jangan menyimpulkan isi dari nama berkas, abstrak, atau daftar isi saja.
2. Catat struktur asli: judul, penulis/lembaga, tahun atau versi, bab/bagian, urutan argumen, istilah kanonik, dan lokasi bukti. Bedakan nomor halaman cetak dari indeks halaman PDF. Bila keduanya berbeda, pilih satu sistem yang jelas dan konsisten pada infografis.
3. Susun lembar kerja internal yang memasangkan setiap calon label atau klaim dengan lokasi sumber yang sudah dilihat. Periksa modalitasnya: rencana, usulan, proses, atau hasil. Jangan mengubah target menjadi capaian. Tandai konflik antarsumber dan minta keputusan pengguna bila dua dokumen otoritatif berbeda makna.
4. Bila pengguna memberi arah, rumuskan satu pertanyaan pengarah. Pilih isi sumber yang menjawabnya tanpa menghilangkan konteks yang mengubah makna. Labeli panel penerapan sebagai `Sintesis` atau `Implikasi`, serta beri catatan singkat bahwa panel itu bukan rekomendasi eksplisit sumber bila memang demikian.

## Rancang peta

1. Tulis dahulu kerangka teks: kondisi awal atau masalah, komponen inti menurut urutan materi, hubungan dan panah yang dapat dibuktikan, prinsip lintas komponen, dan pesan akhir. Gunakan istilah sumber. Jangan menciptakan nama kerangka, kode, atau singkatan baru tanpa persetujuan pengguna.
2. Pilih butir yang cukup untuk satu slide dan dapat dibaca pada layar presentasi. Ringkas dengan parafrasa yang setia. Untuk setiap mekanisme utama, jelaskan tujuan, cara kerja atau kriteria, serta aktor atau periodenya bila sumber menyebutnya. Label tanpa penjelasan belum cukup. Bila sumber terlalu luas, buat beberapa peta sesuai pembagian yang dinyatakan pengguna atau jelaskan cakupan yang dipilih.
3. Cantumkan rujukan **di dekat klaim**: bab, pasal, bagian, halaman cetak, nomor slide, atau timestamp yang benar-benar diperiksa. Footer memuat identitas sumber dan cakupan keseluruhan. Jangan mengarang halaman. Bila lokasi tepat belum dapat dipastikan, tandai untuk verifikasi sebelum merender.
4. Sebelum merancang visual, baca [gaya-visual.md](references/gaya-visual.md) dan **buka gambar `00_genai_framework_ai_driven_university.png`** dengan alat penampil gambar. Itulah satu-satunya acuan visual aktif. Empat gambar lain adalah arsip dan hanya dipakai bila pengguna memintanya. Salin susunan, proporsi, hirarki huruf, garis, ikon, warna, dan posisi sampul gambar `00` setepat mungkin. Sesuaikan isi dan jumlah komponen dengan sumber.
5. Bila sumber mempunyai sampul, tampilkan miniatur sampul yang terbaca sebagai penanda dokumen, seperti pada acuan `00`. Untuk kelompok bernomor, misalnya empat area fokus, beri satu bingkai dan judul yang menyebut jumlahnya. Pastikan setiap anggota kelompok terlihat jelas dan namanya sama dengan sumber.

## Render dan periksa

1. Buat gambar 16:9 berukuran minimal 1920×1080, diutamakan 2880×1620, dengan kisi dan rincian visual pada [gaya-visual.md](references/gaya-visual.md). Untuk presisi teks, gunakan alat vektor, slide, atau raster terprogram; jangan mengandalkan generator gambar untuk tulisan final. Jangan mengirim halaman buku yang dilindungi hak cipta ke repo publik.
2. Buka hasil pada ukuran asli dan bandingkan berdampingan dengan **gambar `00`** pada ukuran tampilan 960×540. Periksa proporsi panel, sampul, font, ikon, warna, garis, dan arah panah. Periksa juga setiap klaim terhadap sumber, terutama judul, nama lembaga, rujukan, isi footer, dan perbedaan rencana dari capaian.
3. Ukur batas setiap teks terhadap kotak atau pita tempatnya berada. Periksa kembali hasil pada 960×540: tidak ada teks keluar, bertabrakan, atau menjadi terlalu kecil; ikon bergaris tetap terlihat; dan sampul tidak berubah proporsi. Gambar panah sebagai bentuk vektor bila font tidak mendukung simbolnya. Perbaiki dan render ulang sampai lolos kedua ukuran.
4. Simpan hasil final di lokasi yang diminta pengguna. Dalam WiraOS, gunakan `_output/` pada scope kerja terdekat. Jangan menimpa versi sebelumnya tanpa permintaan eksplisit. Berikan tautan ke gambar final dan ringkas cakupan, arah sintesis, serta batas bukti yang masih relevan.

## Batas mutu

- Semua isi faktual pada gambar harus terlacak ke sumber yang dibaca. Pengetahuan luar sumber hanya masuk bila diminta, diverifikasi, dan dibedakan jelas.
- Kutipan langsung pendek saja bila perlu; utamakan parafrasa. Patuhi batas hak cipta sumber.
- Jangan memakai label `source of truth`, `berhasil`, `wajib`, atau sejenisnya bila sumber hanya menyebut visi atau usulan.
- Bila materi tidak terbaca, minta versi yang dapat dibaca atau buat peta parsial dengan batas yang terlihat jelas. Jangan mengisi celah dari ingatan.
