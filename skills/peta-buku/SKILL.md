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
2. Pilih butir yang cukup untuk satu slide dan dapat dibaca pada layar presentasi. Ringkas dengan parafrasa yang setia. Bila sumber terlalu luas, buat beberapa peta sesuai pembagian yang dinyatakan pengguna atau jelaskan cakupan yang dipilih.
3. Cantumkan rujukan **di dekat klaim**: bab, pasal, bagian, halaman cetak, nomor slide, atau timestamp yang benar-benar diperiksa. Footer memuat identitas sumber dan cakupan keseluruhan. Jangan mengarang halaman. Bila lokasi tepat belum dapat dipastikan, tandai untuk verifikasi sebelum merender.
4. Untuk gaya infografis, baca [gaya-visual.md](references/gaya-visual.md). Ikuti contoh gambar pengguna bila diberikan. Contoh visual menentukan bahasa desain, sedangkan struktur materi menentukan isi dan jumlah panel.

## Render dan periksa

1. Buat gambar infografis landscape 16:9. Gunakan alat pembuatan gambar yang tersedia untuk visual bergaya ilustratif seperti contoh, atau alat vektor/slide yang memadai bila ketepatan teks dan editabilitas lebih penting. Jika memakai image generator, berikan teks final secara verbatim, hierarki panel, palet, larangan penambahan klaim, dan rujukan gaya. Jangan mengirim halaman buku yang dilindungi hak cipta ke repo publik.
2. Buka hasil pada ukuran asli. Periksa teks satu per satu terhadap kerangka dan sumber, termasuk judul, nama lembaga, nomor rujukan, isi footer, arah panah, potongan kata, dan keterbacaan. Generator gambar dapat mengubah ejaan atau menghilangkan butir. Perbaiki kesalahan terarah lalu periksa ulang. Jika rujukan tidak muat, sederhanakan komposisi atau tambahkan lembar pendamping, jangan mengecilkannya hingga tak terbaca.
3. Simpan hasil final di lokasi yang diminta pengguna. Dalam WiraOS, gunakan `_output/` pada scope kerja terdekat. Jangan menimpa versi sebelumnya tanpa permintaan eksplisit. Berikan tautan ke gambar final dan ringkas cakupan, arah sintesis, serta batas bukti yang masih relevan.

## Batas mutu

- Semua isi faktual pada gambar harus terlacak ke sumber yang dibaca. Pengetahuan luar sumber hanya masuk bila diminta, diverifikasi, dan dibedakan jelas.
- Kutipan langsung pendek saja bila perlu; utamakan parafrasa. Patuhi batas hak cipta sumber.
- Jangan memakai label `source of truth`, `berhasil`, `wajib`, atau sejenisnya bila sumber hanya menyebut visi atau usulan.
- Bila materi tidak terbaca, minta versi yang dapat dibaca atau buat peta parsial dengan batas yang terlihat jelas. Jangan mengisi celah dari ingatan.
