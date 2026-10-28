# Mengaktifkan OpenAI API (Cloudflare Worker)

Backend disiapkan tetapi **belum dideploy**. GitHub Pages hanya menjalankan frontend.

1. Buat API key di https://platform.openai.com/api-keys (API berbayar terpisah dari ChatGPT).
2. Buat akun Cloudflare dan pasang Node.js. Dari folder repository, jalankan `npx wrangler login` dan `npx wrangler deploy`.
3. Tambahkan dua secret ke Worker menggunakan `npx wrangler secret put OPENAI_API_KEY` dan `npx wrangler secret put APP_ACCESS_TOKEN`. Buat APP_ACCESS_TOKEN acak dan kuat; jangan simpan di GitHub. Atau tambahkan melalui Cloudflare Dashboard > Worker > Settings > Variables and Secrets > Add > Secret.
4. Masukkan URL Worker HTTPS di langkah **Validasi & Ekspor** aplikasi. Saat pertama menekan tombol AI, masukkan token akses yang dibuat tadi.
5. Jangan gunakan untuk data sensitif sebelum menambahkan autentikasi institusi, rate limiting, audit, dan kontrol biaya. CORS bukan autentikasi. Token bersama ini hanya cocok untuk uji coba terbatas.

Catatan: Biaya API OpenAI dihitung terpisah. Tidak ada API key atau token di repository. Model default dapat diubah di wrangler.json.
