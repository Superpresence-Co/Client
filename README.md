# Client

Kode final (script & style) untuk website Webflow klien Superpresence.
Satu folder = satu klien. Isinya hanya `script.js` dan `style.css`.

Uji coba dilakukan di CodeSandbox. Kode baru masuk ke sini setelah dikirim ke klien.

> ⚠️ Repo ini **public**. Jangan simpan password, API key, atau catatan internal di sini.

## Daftar klien & kode embed Webflow
Tempel di Webflow → Site settings → Custom code.

### Superpresence V2.5
Folder: `superpresence-v2.5/`

Tempel di **Head**:
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Superpresence-Co/Client@superpresence-v2.5-v1.0.0/superpresence-v2.5/style.css">
```
Tempel sebelum **</body>**:
```html
<script src="https://cdn.jsdelivr.net/gh/Superpresence-Co/Client@superpresence-v2.5-v1.0.0/superpresence-v2.5/script.js" defer></script>
```

### Onelisted V2
Folder: `onelisted-v2/`

Tempel di **Head**:
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Superpresence-Co/Client@onelisted-v2-v1.0.0/onelisted-v2/style.css">
```
Tempel sebelum **</body>**:
```html
<script src="https://cdn.jsdelivr.net/gh/Superpresence-Co/Client@onelisted-v2-v1.0.0/onelisted-v2/script.js" defer></script>
```

## Cara update kode klien
1. Ganti isi `script.js` / `style.css` di folder klien.
2. Commit & push.
3. Buat versi baru, contoh: `git tag onelisted-v2-v1.0.1 && git push --tags`
4. Di Webflow, ganti `v1.0.0` di link embed menjadi versi baru.

Selalu pakai nomor versi di link. Jangan pakai `@main`: perubahan bisa telat muncul (cache sampai 12 jam) dan langsung tayang tanpa dicek.

## Menambah klien baru
Buat folder baru dengan huruf kecil dan tanda `-` (contoh: `nama-klien-v1`), isi `script.js` dan `style.css`, lalu tambahkan kode embed-nya di README ini.
