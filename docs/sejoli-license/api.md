---
sidebar_position: 1
---

# API

API yang disediakan sejoli + addon sejoli license memungkinkan Anda mengaktifkan kode lisensi dari jarak jauh, memeriksa apakah kode tersebut valid (dan tidak kedaluwarsa/expired), dan juga mengambil informasi tentang versi plugin/theme/app. API ini dapat diimplementasikan dengan sebagian besar perangkat lunak/app, bukan hanya Plugin dan Theme WordPress.


## Permintaan API yang tersedia

- `activation_license` → Digunakan untuk mengaktifkan kode lisensi dari jarak jauh
- `deactivate_license` → Digunakan untuk menonaktifkan kode lisensi dari jarak jauh
- `check_license` → Digunakan untuk memeriksa dari jarak jauh apakah kode lisensi diaktifkan, valid, dan tidak kedaluwarsa
- `get_version` → Digunakan untuk mengambil informasi versi terbaru suatu produk dari jarak jauh

Masing-masing metode di bawah ini bekerja dengan cara yang sama. URL situs web tempat Anda menginstal plugin Sejoli + Sejoli License Manage akan bertindak sebagai titik akhir API. Semua permintaan ke API dilakukan sebagai permintaan GET atau POST dan ikuti formulir ini:

```bash
https://YOURSITE.com/?sejoli_action={request type}&item_name={slug product}&license=0000072651-CCS5T-TNZ1L-JEXN3-1O0CSD&url={url of the site being licensed}
```

Build your site **for production**:

```bash
npm run build
```

The static files are generated in the `build` folder.

## Deploy your site

Test your production build locally:

```bash
npm run serve
```

The `build` folder is now served at [http://localhost:3000/](http://localhost:3000/).

You can now deploy the `build` folder **almost anywhere** easily, **for free** or very small cost (read the **[Deployment Guide](https://docusaurus.io/docs/deployment)**).
