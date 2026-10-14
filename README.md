# Misi Nombor — Matematik Darjah 1

Permainan sasaran angkasa Bahasa Melayu. 12 soalan tambah dan tolak hingga 20, termasuk masalah harian dan soalan pemindahan kefahaman. Tempoh anggaran 5–10 minit. Tiada pemasa, backend, pemasangan atau aset luar.

## Struktur
```
math-darjah-1/
  index.html
  style.css
  script.js
  README.md
```
Grafik menggunakan CSS dan emoji sistem. Rupa emoji mungkin berbeza antara peranti.

## Uji secara lokal
Ekstrak ZIP terlebih dahulu. Buka index.html dalam Chrome, Edge, Firefox atau Safari. Jangan buka HTML dari dalam ZIP. Semua tiga fail kod mesti berada dalam folder yang sama.

## Kawalan dan skor
Klik atau sentuh sasaran, atau tekan 1/2/3. Tab dan Enter juga berfungsi. Gerakan sasaran boleh dimatikan di halaman utama. Jawapan betul pada cubaan pertama mendapat satu bintang. Jawapan salah memberi petunjuk dan peluang cuba semula. Tiada bonus kelajuan. Teruskan hanya tersedia selepas jawapan betul. Mula semula dan Utama menamatkan sesi semasa; data tidak disimpan.

## GitHub Pages
1. Cipta repository bernama math-darjah-1 (pilih Public jika menggunakan GitHub Free).
2. Pilih Add file → Upload files.
3. Muat naik ISI folder: index.html, style.css, script.js, README.md. Jangan muat naik ZIP atau folder induk sebagai satu subfolder.
4. Commit changes.
5. Buka Settings → Pages → Build and deployment.
6. Pilih Source: Deploy from a branch, Branch: main, folder: /(root), kemudian Save.
7. Tunggu deployment selesai. Buka URL yang GitHub paparkan, biasanya https://USERNAME.github.io/math-darjah-1/.
Jika 404, semak index.html huruf kecil berada di root branch main dan deployment telah siap. Tetapan akaun/organisasi mungkin mengehadkan Pages.
Rujukan: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Edit soalan
Buka script.js dan edit QUESTIONS di bawah BANK SOALAN BOLEH DIEDIT. Setiap soalan mempunyai topic, text, options (tiga nilai nombor unik), answer (nilai jawapan yang betul), explain, hint. Jangan gunakan indeks pilihan sebagai answer. Progress dan jumlah skor disesuaikan secara automatik. Kekalkan soalan baharu untuk semak kefahaman sebagai soalan terakhir. Ubah teks tempoh/bilangan pada homepage jika bilangan soalan berubah. Visual titik bagi soalan pertama dalam render() perlu diubah jika soalan pertama berubah.
Contoh:
```js
{topic:'Tambah',text:'3 + 2 = ?',options:[4,5,6],answer:5,
 explain:'3 ditambah 2 menjadi 5.',hint:'Kira dua langkah selepas 3.'}
```

## Semakan dan batas ujian
Lulus semakan sintaks JavaScript dan ujian logik dengan DOM simulasi: mula, jawapan salah, cuba lagi, pengiraan sekali sahaja, 12 soalan, tamat, mula semula, kembali utama dan bank jawapan.
Ujian visual dalam browser sebenar tidak dijalankan dalam persekitaran ini. Ujian simulasi tidak membuktikan susun atur atau sentuhan sebenar.

### Checklist manual sebelum kelas
- Buka index.html; Cara bermain dan Mula misi berfungsi.
- Klik jawapan salah, baca petunjuk, tekan Cuba lagi; kemudian pilih betul.
- Klik berulang semasa feedback: skor kekal.
- Gunakan 1/2/3, Tab/Enter dan sentuhan telefon.
- Selesaikan 12 soalan; semak skor dan penerangan setiap soalan.
- Mula semula: skor kembali 0; Utama: kembali homepage.
- Matikan gerakan sasaran dan cuba lagi.
- Semak lebar 360px, 768px dan desktop, serta zoom 200%: soalan dan tiga sasaran dapat dibaca tanpa pertindihan.
- Uji URL GitHub Pages di komputer dan telefon selepas deployment.
