# RootCause Windows Inspector — Landing Page

Página web pública del producto [RootCause Windows Inspector](https://github.com/vladimiracunadev-create/rootcause-windows-inspector).

🌐 **Ver online:** https://vladimiracunadev-create.github.io/rootcause-landing

---

## Estructura

```
rootcause-landing/
├── index.html              ← página principal
├── assets/
│   ├── style.css           ← estilos (dark theme, sin dependencias)
│   └── favicon.svg         ← ícono SVG
└── .github/
    └── workflows/
        └── deploy.yml      ← auto-deploy a GitHub Pages en cada push
```

## Deploy

El workflow `.github/workflows/deploy.yml` despliega automáticamente a GitHub Pages en cada push a `main`.

Para activarlo la primera vez:
1. Ve a **Settings → Pages** del repo
2. En **Source** selecciona **GitHub Actions**
3. El siguiente push a `main` desplegará la página

## Notas

- Este repo es **público** para poder usar GitHub Pages gratis.
- El código fuente del producto vive en el repo **privado** `rootcause-windows-inspector`.
- Cuando el repo del producto sea público, la landing puede integrarse como rama `gh-pages` o mantenerse separada.
