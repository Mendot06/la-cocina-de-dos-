# La Cocina de Dos

Sitio web estático de un emprendimiento familiar (madre e hijo/a) que vende **tartas** (verdura, jamón y queso, pollo y puerro) y **sanguches** (jamón y queso, salame y queso).
## Tecnologías

HTML5 semántico · SCSS (arquitectura de partials) · Bootstrap 5.3 (CDN) · AOS (animaciones al scroll) · SEO on-page · Vercel / Netlify

## Estructura

```
index.html
pages/            tartas.html · sanguches.html · nosotros.html · contacto.html
scss/             main.scss (solo @use) + utilities/ base/ layout/ components/ pages/
styles/           main.css (compilado)
assets/img/       ilustraciones y logo (SVG)
js/main.js        AOS + formulario que abre WhatsApp
robots.txt · sitemap.xml
```

## Compilar los estilos

```bash
npm install
npm run sass          # compila una vez
npm run sass:watch    # compila al guardar
```

## Cosas para personalizar antes de publicar

1. **WhatsApp:** reemplazá `5491100000000` / `+54 9 11 0000-0000` en los HTML y en `js/main.js`.
2. **Dominio:** reemplazá `https://la-cocina-de-dos.vercel.app` por tu URL real en los `<link rel="canonical">`, `robots.txt` y `sitemap.xml`.
3. **Fotos:** las imágenes son ilustraciones. Podés reemplazarlas por fotos reales en `assets/img/` (mantené nombres descriptivos y actualizá los `alt`).
4. **Textos:** horarios, zona de entrega y preguntas frecuentes son genéricos; ajustalos a la realidad del emprendimiento.

## Subir a GitHub (desde la consola)

```bash
git init
git add .
git commit -m "Estructura base del sitio: HTML semántico y navbar de Bootstrap"
git add .
git commit -m "Estilos SCSS con partials, animaciones y SEO"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/la-cocina-de-dos.git
git push -u origin main
```
