# Gus Portfolio

Portafolio de Gustavo Zschommler — UX/UI Designer. Construido a partir del sistema de diseño **Gus Design System v1.1** en Figma (tokens actualizados: Electric Violet `#7951E9`, tipografía Inter + Lora + DM Mono).

Sitio 100% estático: **HTML + CSS + JS**, sin build ni dependencias.

## Estructura

```
index.html            → Home
about.html            → About Me (work history, skills, education)
case-alma.html        → Case study: Alma
case-sportstech.html  → Case study: Sportstech
case-ourspace.html    → Case study: OurSpace (identidad propia dark + lime)
case-photo-3d.html    → Case study: Photo + 3D Manipulation
case-ads.html         → Case study: Display Advertising
css/
  tokens.css          → Design tokens (colores, tipografía, espaciado, radios, sombras)
  base.css            → Reset, tipografía, navbar, footer, botones, chips
  home.css, about.css, case.css, sportstech.css, ourspace.css, photo3d.css, ads.css
assets/img/           → Imágenes e iconos exportados de Figma
```

## Ver en local

```bash
npx serve .          # o: python3 -m http.server 8000
```

## Conectar a un dominio (deploy)

Cualquier hosting estático funciona. Los tres más fáciles (gratis):

**Vercel** (recomendado)
1. `npm i -g vercel && vercel` dentro de esta carpeta (o arrastra la carpeta en vercel.com/new).
2. En el dashboard: Settings → Domains → añade tu dominio.
3. En tu proveedor de dominio, apunta el DNS: registro `A` a `76.76.21.21` o `CNAME` a `cname.vercel-dns.com`.

**Netlify**
1. Arrastra la carpeta en app.netlify.com/drop.
2. Domain settings → Add custom domain → sigue las instrucciones de DNS.

**GitHub Pages**
1. Sube la carpeta a un repo y activa Pages (Settings → Pages → branch `main`).
2. Añade tu dominio en "Custom domain" y crea el registro `CNAME` en tu DNS.

## Breakpoints

- Desktop: > 1100px (diseño base 1440)
- Tablet: ≤ 1100px (diseño 834)
- Mobile: ≤ 640px (diseño 402)
