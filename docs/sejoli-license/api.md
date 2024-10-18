---
sidebar_position: 1
---

# Deploy your site

API yang disediakan sejoli + addon sejoli license memungkinkan Anda mengaktifkan kode lisensi dari jarak jauh, memeriksa apakah kode tersebut valid (dan tidak kedaluwarsa/expired), dan juga mengambil informasi tentang versi plugin/theme/app. API ini dapat diimplementasikan dengan sebagian besar perangkat lunak/app, bukan hanya Plugin dan Theme WordPress.


## Build your site

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
