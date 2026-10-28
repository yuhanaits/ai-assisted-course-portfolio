# AI-Assisted Course Portfolio System (AI-CPS)

Prototipe web statis untuk workflow penyusunan portofolio mata kuliah berbasis OBE.

## Fitur
- Input identitas mata kuliah, CPL, dan CPMK
- Draf RPS 16 minggu berbasis template
- Contoh asesmen dan rubrik
- Pemeriksaan kelengkapan
- Catatan validasi dan ekspor TXT/JSON
- Penyimpanan lokal di browser

**Batasan:** Belum menggunakan AI generatif, belum memiliki autentikasi, database bersama, atau approval yang terverifikasi. Jangan masukkan data pribadi mahasiswa maupun dokumen rahasia. Konten keluaran adalah draf dan wajib diperiksa dosen.

## Deploy
Settings → Pages → Deploy from a branch → main / (root) → Save.

## Integrasi AI berikutnya
Gunakan backend serverless dengan secret API key di sisi server, kontrol akses, audit trail, dan pemrosesan dokumen sesuai kebijakan institusi. Jangan menaruh API key pada JavaScript browser atau repository publik.
