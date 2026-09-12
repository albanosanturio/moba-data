# moba — landing page

Sitio estático, sin backend propio.

## Estructura

```
/index.html          página en español (default)
/en/index.html        página en inglés
/styles.css           estilos compartidos
/images/               fondo del hero (desktop + versión mobile)
/fonts/                Space Grotesk, Inter, IBM Plex Mono (woff2, autohospedadas)
/icons/                moba-icon.svg, favicons, og-image.png
```

## El fondo del hero

`images/hero-bg.jpg` (y su versión `hero-bg-mobile.jpg` para pantallas chicas)
se usa como fondo de la sección hero vía CSS `background-image`, con un
degradé que lo funde hacia el carbón de la marca para que el texto quede
legible sobre el lado izquierdo. Es una imagen estática, sin JS ni
animación.

## Deploy

Cualquier hosting estático sirve (Vercel, Netlify, Cloudflare Pages, GitHub
Pages): apuntar la raíz del deploy a esta carpeta. No requiere build step.

## Dominio

`mobadata.net`. Ya aplicado en meta tags, hreflang, og:image y los mails de
contacto de ambos footers.

## Pendiente antes de publicar

- **Analítica**: no está incluida. Agregar Plausible o Umami (script
  liviano, sin cookies) antes de publicar si se quiere medir tráfico.
- **WHOIS**: verificar que la privacidad de WHOIS esté activada en
  Namecheap para el registro de `mobadata.net`.
- **DNS**: apuntar el dominio al hosting elegido (ver sección Deploy)
  desde el panel de Namecheap.

## Checklist de marca ya aplicado

- Sin nombres de personas, fotos ni biografías en ningún lado.
- Mail de contacto genérico (`hola@dominio`), no personal.
- `meta author` ausente; sin comentarios de autor en el código.
- Rojo (`#E63946`) usado solo como acento (CTAs, marcadores, algunos
  puntos de la imagen de fondo), nunca como fondo de sección completa.
- "moba" en minúscula en el sitio; "Moba" con mayúscula inicial reservado
  para texto corrido si hiciera falta en algún documento aparte.
- Tipografías autohospedadas, sin llamadas a Google Fonts.
