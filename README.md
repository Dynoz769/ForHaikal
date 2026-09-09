# Surat Untuk Haikal

Satu halaman kenang-kenangan untuk adik aku, Haikal, yang mula belajar di UPSI
(Universiti Pendidikan Sultan Idris, Tanjung Malim) pada **Jumaat, 11 September 2026**.

Aku tak dapat berada di sana hari dia bertolak. Jadi aku buat benda ni.

## Isi halaman

| Bahagian | Apa dia |
|---|---|
| **Pintu masuk** | Skrin hitam dengan butang `For My Universe`. Tekan → intro ala Netflix di atas canvas: berkas cahaya merah memancar keluar dari tengah, dan setiap jalur mengecat sekeping nama `HAIKAL` bila ia sampai. Bunyi *ta-dum* disintesis dengan WebAudio (bukan fail audio). ~3.2 saat, ada butang **Langkau**. |
| **Kiraan detik** | Hari / jam / minit / saat sampai 11 September 2026, 8:00 pagi waktu Malaysia. Lepas tarikh tu berlalu, dia bertukar sendiri jadi kiraan "hari sejak kau bertolak". |
| **Surat** | Enam perenggan dalam Bahasa Melayu. |
| **Surat berkunci** | Tiga sampul bermeterai: rindu rumah, bila rasa nak mengalah, dan hari dia jadi cikgu. Dibuka satu-satu; halaman ingat mana yang dah dibuka melalui `localStorage`, jadi rekod tu peribadi kepada dia sahaja. |
| **Album** | Lapan gambar terbenam terus dalam `index.html` sebagai data URI, jadi ia muncul di mana-mana halaman ni dibuka. Salinan asal ada dalam `gambar/`. Gambar tambahan yang dimuat naik melalui halaman disimpan dalam pangkalan data artifact dan muncul selepas lapan yang tetap tu. |
| **Lagu** | *Kita Lewati Berdua* — Overnight, terbenam dalam `index.html` sebagai data URI (3:59, 123 kbps). Mula bila butang pintu ditekan (tekanan tu yang benarkan browser main bunyi), pudar masuk selepas *ta-dum*, dan berulang. Butang senyap kekal di penjuru bawah kanan; pilihan disimpan dalam `localStorage`. Fail asal ada dalam `lagu/`. |
| **Penamat** | Bila bahagian penutup masuk pandangan: kilat berkelip dua kali, ayat terakhir muncul putih menyilau lepas tu turun ke warna sebenarnya, guruh bergolek (bunyi rawak ditapis rendah, senyap kalau lagu disenyapkan), semua air pada skrin gugur serentak, dan laluan Rumah-Tanjung Malim-UPSI dijejaki cahaya satu per satu. |
| **Suasana** | Butang tukar antara palet *Subuh* (cerah) dan *Malam* (gelap). Ikut tema peranti kalau tak disentuh. |

## Nota teknikal

Satu fail `index.html` — tiada langkah bina, tiada kebergantungan. Fon dari Google Fonts
(Bebas Neue, Fraunces, Karla, IBM Plex Mono); semua CSS dan JS ada dalam fail.

**Album tu perlukan runtime Claude Artifacts.** Halaman ni memanggil
`claude.use("db")` untuk baca dan simpan gambar. Buka fail ni terus dari cakera atau
dari GitHub Pages, dan bahagian lain berfungsi seperti biasa manakala album tu papar
"Album tak tersedia di sini" — memang begitu direka, bukan pepijat. Kebenaran album:
baca untuk sesiapa yang boleh buka, tulis untuk editor sahaja.

Air menitik di latar dan intro dilukis atas `<canvas>`.

Halaman ini sengaja TIDAK menghormati `prefers-reduced-motion`. Windows yang
matikan kesan animasi (MinAnimate = 0) buat Chrome melaporkan tetapan tu, dan
dulu ia membekukan intro serta seluruh peralihan CSS pada mesin pemilik halaman
ini. Gerakan di sini lembut dan tidak memenuhi skrin, jadi gerbang tu dibuang.

## Di mana halaman ini hidup

Diterbitkan sebagai Claude Artifact (private):
<https://claude.ai/code/artifact/3e0525ba-b9c5-4c16-84e5-2cf2f2e397ae>

Repo ni salinan sumbernya. Untuk mengubah halaman yang Haikal buka, artifact tu yang
kena diterbitkan semula — bukan cukup dengan push ke sini.
