# Tayangan Sejarah bersuara — pakej hosting
## Mula
Buka index.html. Pilih Autoplay atau Manual. Pilihan ini meminta fullscreen dan membuka audio melalui klik pengguna. Jika pelayar menolak fullscreen, tayangan tetap berjalan dan butang Skrin penuh tersedia. iPhone/pelayar tertentu mengehadkan fullscreen.

Autoplay: 21:40.9 termasuk semua audio, 7 saat selepas MCQ, 1 saat selepas setiap halaman isi dan transition. MP3 dimainkan pada kadar 1.1×. Kelajuan rangkaian atau jeda boleh menambah masa. Manual: transition → audio → menunggu Next. Menu dan pertukaran tab menjedakan tayangan. Papar jawapan menjedakan tayangan dan membacakan jawapan.

## Hosting
Muat naik SELURUH kandungan folder ini, mengekalkan struktur asal. Entry guru: index.html. Entry murid: jawapan-murid.html. Fail audio/, transition/, PNG/JPG diperlukan. Semua aset adalah tempatan; tiada API key, CDN atau akaun Microsoft diperlukan untuk memainkan MP3. Gunakan hosting statik melalui HTTPS. Pastikan MP3 dilayan sebagai audio/mpeg dan nama fail peka huruf besar/kecil tidak berubah. Jangan muat naik index.html sahaja.

## Respons murid
Fail jawapan murid berasingan menyimpan respons serta markah secara automatik dalam pelayar pada peranti murid. Selepas Hantar jawapan, murid melihat jumlah betul dan salah. Butang muat turun dan cetak telah dibuang. Tiada penghantaran automatik atau Firebase. Guru mempunyai kunci dalam fail guru dan skrip; edarkan pautan murid sahaja kepada murid.

## Fail
index.html dan index-RAW.txt; jawapan-murid.html dan RAW; 43 MP3 dalam audio/; audio-manifest.json dengan teks, suara dan durasi asal; transition/; ilustrasi PNG/JPG; prompt imej; SKRIP_DAN_TIMING.md; README.md. Tiada proses build diperlukan pada hosting.

## Sumber dokumentasi sahaja
Buku teks Sejarah KSSM Tingkatan 3, Bab 1.1, halaman 4–5 dan 8–9. Ilustrasi ialah gambaran rekaan pendidikan. Audio dijana menggunakan Microsoft Edge online TTS melalui edge-tts, disimpan sebagai fail MP3; bukan panggilan Azure ketika tayangan.

## Semakan penyegerakan
Highlight menggunakan lima cue daripada timestamp perkataan sebenar dalam setiap narasi. Cue disertakan dalam audio-manifest.json dan HTML. Metadata perkataan asal disimpan dalam sync/. Jam tayangan menunjukkan masa aktif sebenar. Jumlah nominal 21:40.947, dipaparkan sebagai anggaran 21:41. Audio 19:22.647 + sela MCQ 1:10 + jeda isi 0:20 + transition 0:48.3. Loading boleh menambah masa. Label kurikulum dan sumber dibuang daripada paparan; rujukan dikekalkan dalam dokumentasi.
