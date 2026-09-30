# School Portal API Documentation

Dokumentasi API berbasis OpenAPI 3.0.3 untuk School Portal yang terintegrasi dengan Odoo ERP.

## Struktur

- `openapi.yaml` — single source of truth API contract.
- `index.html` — renderer dokumentasi berbasis Scalar.

## Menjalankan lokal

Jangan membuka `index.html` langsung dengan `file://` karena browser dapat memblokir pemuatan `openapi.yaml`. Jalankan static server, misalnya:

```bash
python -m http.server 8080
```

Kemudian buka `http://localhost:8080`.

## Deploy GitHub Pages

Upload `index.html` dan `openapi.yaml` ke repository GitHub, lalu aktifkan GitHub Pages dari branch/folder repository tersebut. Setelah deploy, bagikan URL Pages kepada anggota tim.

## Catatan

URL `servers` di OpenAPI tetap mengikuti kontrak API yang sudah dibuat. URL dokumentasi (GitHub Pages) berbeda dengan URL server API.
