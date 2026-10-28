# Minecraft Bedrock Sound Preview

**English** | [Bahasa Indonesia](#bahasa-indonesia)

A small website for listening to Minecraft Bedrock Edition sounds, so you can find out exactly which sound file to replace in your own resource pack.

**Website:** https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/

> Vanilla Bedrock sounds are stored as `.fsb` files, which normal audio players (especially on phones) can't open. This site offers short MP3 previews of them, organized in the same folders as the game.

---

## How to replace a sound

1. **Find the sound.** Open the website, type a keyword (for example `villager hurt`), and tap ▶ to listen. The length of each clip is shown next to its folder.
2. **Copy the path.** Tap **Copy**. It copies the folder and file name without an extension, for example `sounds/mob/villager/hurt1`.
3. **Convert your own audio to OGG.** Minecraft needs `.ogg` files. You can use:
   - an online converter such as <https://audio.online-convert.com/convert-to-ogg>
   - Audacity (PC): File → Export → Export as OGG
   - ffmpeg: `ffmpeg -i your_sound.mp3 -c:a libvorbis your_sound.ogg`
4. **Rename it** to the copied name and add `.ogg`, for example `hurt1.ogg`.
5. **Put it in the same folder inside your resource pack**, for example:

   ```
   YourPack/
   ├── manifest.json
   └── sounds/
       └── mob/
           └── villager/
               └── hurt1.ogg
   ```
6. Apply the pack and trigger the sound in the game to test it.

### Good to know

- **OGG works. MP3 does not.** A correctly named `.ogg` file replaces the vanilla sound. An `.mp3` with the same name did not. Other formats (such as `.wav`) have not been tested.
- Some sounds have several variants (for example `hurt1`, `hurt2`). Replace each variant you want to change.
- Previews named like `name_1`, `name_2` come from a sound bank that contains several sounds. <!-- TODO: confirm in-game which file name a replacement needs for banks with several sounds, then state it here. -->
- The preview clips are low-quality MP3s made only for listening. Don't use them in your pack.

---

## Credits and disclaimer

Minecraft and all its sounds belong to Mojang Studios / Microsoft. These short clips are provided only as previews to help people make resource packs. This project is not affiliated with or endorsed by Mojang or Microsoft. If you are a rights holder and want something removed, please open an issue.

For the official vanilla resource files, see Mojang's [bedrock-samples](https://github.com/Mojang/bedrock-samples) repository.

---

<a id="bahasa-indonesia"></a>

# Pratinjau Suara Minecraft Bedrock

[English](#minecraft-bedrock-sound-preview) | **Bahasa Indonesia**

Situs kecil untuk mendengarkan suara Minecraft Bedrock Edition, supaya kamu tahu persis file suara mana yang ingin diganti di resource pack buatanmu sendiri.

**Situs:** https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/

> Suara bawaan Bedrock disimpan dalam file `.fsb` yang tidak bisa dibuka pemutar audio biasa (terutama di HP). Situs ini menyediakan pratinjau MP3 singkat dengan susunan folder yang sama seperti di dalam game.

---

## Cara mengganti suara

1. **Cari suaranya.** Buka situs, ketik kata kunci (contoh: `villager hurt`), lalu ketuk ▶ untuk mendengarkan. Durasi tiap klip ditampilkan di samping nama foldernya.
2. **Salin path-nya.** Ketuk **Copy**. Yang tersalin adalah folder dan nama file tanpa ekstensi, misalnya `sounds/mob/villager/hurt1`.
3. **Ubah audiomu menjadi OGG.** Minecraft membutuhkan file `.ogg`. Kamu bisa memakai:
   - konverter online seperti <https://audio.online-convert.com/convert-to-ogg>
   - Audacity (PC): File → Export → Export as OGG
   - ffmpeg: `ffmpeg -i suaramu.mp3 -c:a libvorbis suaramu.ogg`
4. **Ganti namanya** sesuai nama yang disalin dan tambahkan `.ogg`, misalnya `hurt1.ogg`.
5. **Taruh di folder yang sama di dalam resource pack-mu**, contohnya:

   ```
   PackKamu/
   ├── manifest.json
   └── sounds/
       └── mob/
           └── villager/
               └── hurt1.ogg
   ```
6. Aktifkan pack-nya, lalu pancing suara tersebut di dalam game untuk mengetesnya.

### Perlu diketahui

- **OGG berhasil, MP3 tidak.** File `.ogg` dengan nama yang benar akan menggantikan suara bawaan. File `.mp3` dengan nama yang sama tidak berfungsi. Format lain (seperti `.wav`) belum diuji.
- Beberapa suara punya beberapa variasi (misalnya `hurt1`, `hurt2`). Ganti setiap variasi yang ingin kamu ubah.
- Pratinjau dengan nama seperti `nama_1`, `nama_2` berasal dari satu bank suara yang berisi beberapa suara. <!-- TODO: pastikan di dalam game nama file apa yang dipakai untuk bank berisi beberapa suara, lalu tulis di sini. -->
- Klip pratinjau berupa MP3 berkualitas rendah yang dibuat hanya untuk didengarkan. Jangan dipakai di pack-mu.

---

## Kredit dan pernyataan

Minecraft dan semua suaranya adalah milik Mojang Studios / Microsoft. Klip singkat ini hanya disediakan sebagai pratinjau untuk membantu pembuatan resource pack. Proyek ini tidak berafiliasi dengan atau didukung oleh Mojang maupun Microsoft. Jika kamu pemegang hak cipta dan ingin sesuatu dihapus, silakan buka issue.

Untuk file resource resmi bawaan, lihat repositori [bedrock-samples](https://github.com/Mojang/bedrock-samples) dari Mojang.