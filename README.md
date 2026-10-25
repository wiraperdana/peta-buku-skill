# peta-buku-skill

Skill Agent untuk membuat infografis landscape dari kerangka dan alur isi buku, slide, serta materi lain yang dapat dibaca. Setiap klaim dirujuk ke bagian sumber. Pengguna juga dapat memberi arah penerapan tertentu; implikasi dari agent diberi label sebagai sintesis.

## Pakai

Di Claude Code: `/peta-buku <lampiran atau path> [arah yang diinginkan]`.

Di Codex dan agent lain: `Pakai skill $peta-buku untuk membuat infografis dari <lampiran atau path>. Arahkan ke <topik>.`

Contoh: `Pakai $peta-buku untuk buku ini. Petakan pengalaman reformasi arsitektur digital dan tarik pelajaran bagi AI Policy Kemenkeu.`

Skill dapat membaca PDF, PPT/PPTX, Markdown, DOCX, gambar, dan format lain sepanjang lingkungan agent menyediakan pembaca atau OCR yang sesuai. Hasil gambar membutuhkan alat pembuat gambar atau slide yang tersedia di lingkungan tersebut.

## Pasang

```bash
git clone https://github.com/wiraperdana/peta-buku-skill.git
cd peta-buku-skill
./install.sh
```

`install.sh` membuat symlink ke `~/.claude/skills/peta-buku` dan `~/.agents/skills/peta-buku`. Perubahan di repo langsung terbaca oleh kedua harness. Untuk menghapus pemasangan, hapus dua symlink itu secara manual.

Repo ini memuat instruksi skill dan lima contoh visual pada `skills/peta-buku/references/`. Gambar `00_genai_framework_ai_driven_university.png` adalah satu-satunya acuan visual aktif. Empat lainnya disimpan sebagai arsip dan dipakai hanya bila pengguna memintanya. Contoh visual bukan sumber isi untuk tugas lain. Materi sumber dan infografis hasil tugas tetap berada di lokasi kerja pengguna.

## Lisensi

MIT, lihat [LICENSE](LICENSE).
