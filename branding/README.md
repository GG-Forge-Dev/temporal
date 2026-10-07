# Partii — kit de marca

Logo de Partii escalado con superresolución (EDSR ×4) a partir del original de 384×256,
más favicons e íconos de app listos para usar.

## Contenido

| Carpeta | Archivos | Uso |
|---|---|---|
| `logo/` | `partii-logo-{2048,1536,1024,512,256}…png` | Logo completo sobre fondo negro |
| `logo/` | `partii-logo-transparent-…png` | Logo con fondo transparente (para fondos oscuros) |
| `logo/` | `partii-logo-light-bg-…png` | Fondo transparente con el texto "Part" oscuro (para fondos claros) |
| `logo/` | `partii-logo-square-{1024,512}.png` | Logo completo en lienzo cuadrado (negro o transparente) |
| `icon/` | `partii-icon-{1024,512,256,128,64}.png` | Ícono de la app (la "P" con el control) sobre negro |
| `icon/` | `partii-icon-transparent-…png` | Ícono de la app con fondo transparente |
| `favicon/` | `favicon.ico` (16/32/48/64), `favicon-16x16.png`, `favicon-32x32.png`, `favicon-48x48.png` | Favicon del sitio |
| `favicon/` | `apple-touch-icon.png` (180), `android-chrome-192x192.png`, `android-chrome-512x512.png`, `maskable-icon-512x512.png`, `mstile-150x150.png`, `site.webmanifest` | iOS, Android / PWA, Windows |
| `social/` | `og-image-1200x630.png`, `twitter-header-1500x500.png`, `banner-1920x1080.png`, `profile-400x400.png` | Redes sociales y vista previa de enlaces |
| `source/` | `partii-original-384x256.png` | Imagen original |

Para App Store / Google Play usa `icon/partii-icon-1024.png` (las tiendas exigen fondo opaco).

## Instalación en la web

Copia el contenido de `favicon/` a la raíz pública de tu sitio (`public/` en Vite, Next.js, etc.)
y agrega esto dentro de `<head>`:

```html
<link rel="icon" href="/favicon.ico" sizes="any">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
<link rel="apple-touch-icon" href="/apple-touch-icon.png">
<link rel="manifest" href="/site.webmanifest">
<meta name="theme-color" content="#000000">
<meta property="og:image" content="/og-image-1200x630.png">
```

En Expo / React Native: `icon` → `icon/partii-icon-1024.png`, `adaptiveIcon.foregroundImage`
→ `icon/partii-icon-transparent-1024.png` con `backgroundColor: "#000000"`.
