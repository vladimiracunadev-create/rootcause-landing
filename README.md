# RootCause Windows Inspector — Landing Page

Página web pública del producto [RootCause Windows Inspector](https://github.com/vladimiracunadev-create/rootcause-windows-inspector).

🌐 **Ver online:** https://vladimiracunadev-create.github.io/rootcause-landing

**Versión actual:** v0.7.0

---

## Estructura

```
rootcause-landing/
├── index.html              ← página principal (hero, features, editions, CLI, download)
├── assets/
│   ├── style.css           ← estilos (dark theme, sin dependencias)
│   └── favicon.svg         ← ícono SVG
└── .github/
    └── workflows/
        └── deploy.yml      ← auto-deploy a GitHub Pages en cada push a main
```

## Secciones de la landing

| Sección | Ancla | Descripción |
|---|---|---|
| Hero | — | Título, badges, botón de descarga |
| Características | `#features` | 12 cards con features del producto |
| Ediciones | `#editions` | 6 ediciones: GUI, CLI-only, PowerShell, VS Code, Tray, Service |
| Pestañas | — | Tabla de las 8 pestañas de la GUI |
| Requisitos | `#requirements` | Mínimos, recomendados, modo precisión |
| Instalación | `#install` | Instalador, gestores de paquetes, módulo PowerShell |
| CLI | `#cli` | Referencia de comandos + demo terminal |
| Atajos | — | Tabla de atajos de teclado |
| Descargar | `#download` | 4 tarjetas: Setup, CLI-only ZIP, PowerShell, Licencia |

## Deploy

El workflow `.github/workflows/deploy.yml` despliega automáticamente a GitHub Pages en cada push a `main`.

Para activarlo la primera vez:
1. Ve a **Settings → Pages** del repo
2. En **Source** selecciona **GitHub Actions**
3. El siguiente push a `main` desplegará la página

## Releases y descargas

Los botones de descarga apuntan a:
```
https://github.com/vladimiracunadev-create/rootcause-landing/releases/latest
```

Para que funcionen, publicar los binarios como release en este repo con los siguientes artefactos:
- `rootcause-windows-inspector-setup.exe` — instalador GUI
- `rootcause-windows-x64.zip` — CLI-only portable
- `RootCause.psm1` — módulo PowerShell

## Notas

- Este repo es **público** para poder usar GitHub Pages gratis.
- El código fuente del producto vive en el repo **privado** `rootcause-windows-inspector`.
- Telemetría: cero — verificable en `Cargo.toml` del producto (sin crates de red).
