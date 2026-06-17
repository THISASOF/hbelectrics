# ⚡ HBelectrics — Sitio Web Corporativo

Sitio web de alta conversión para **HBelectrics**, empresa de servicios eléctricos en Bogotá, Colombia. HTML/CSS/JS puro — sin frameworks, sin dependencias, un solo archivo por página.

---

## Vista previa

| Landing principal | Coming Soon |
|---|---|
| `index.html` | `hbelectrics-coming-soon.html` |
| Landing de ventas con formulario → WhatsApp | Página de pre-lanzamiento con countdown y captura de leads |

---

## Stack

- **HTML5** semántico
- **CSS3** con variables CSS nativas
- **JavaScript vanilla** — sin jQuery, sin frameworks
- **Google Fonts** — Bebas Neue (títulos) + Nunito (cuerpo)
- **Google Analytics** (GA4) integrado
- Archivo único por página — sin build step, sin bundler

---

## Páginas

### `index.html` — Landing principal
Landing de alta conversión optimizada para SEO local (Bogotá). Incluye:

- Hero con formulario de cotización → WhatsApp directo
- Barra de trust (RETIE, SENA alturas, garantía escrita, 60 min respuesta)
- 6 servicios: cortocircuitos, instalaciones, cableado, CCTV, redes WiFi/LAN, industrial
- Galería de trabajos (grid masonry con hover overlay)
- Sección de videos de proyectos
- 3 testimonios de clientes reales
- Botón WhatsApp flotante con animación pulsante
- Meta tags SEO completos (Open Graph, Twitter Cards, geo tags)

### `hbelectrics-coming-soon.html` — Coming Soon
Página de pre-lanzamiento minimalista. Incluye:

- Countdown regresivo configurable
- Formulario de captura de leads → WhatsApp
- CTAs de contacto directo (llamar / WhatsApp)
- Barra de trust compacta

---

## Personalización rápida

### Cambiar fotos de la galería
En `index.html`, buscar las etiquetas `<img>` dentro de `.gitem`:

```html
<!-- Reemplazar URL de placeholder por foto real -->
<img src="./fotos/tablero-chapinero.jpg" alt="Instalación tablero Chapinero"/>
```

### Agregar video de YouTube
En `index.html`, al final del script:

```javascript
const VIDEO_ID = 'ABC123xyz'; // ID del video de YouTube
```

### Ajustar fecha del countdown
En `hbelectrics-coming-soon.html`:

```javascript
const TARGET_DATE = new Date('2025-12-31T00:00:00');
```

---

## Contacto embebido

Todos los CTAs apuntan a:

```
WhatsApp:  https://wa.me/573019062800
Llamada:   tel:3019062800
```

---

## Identidad de marca

| Token CSS | Hex | Uso |
|---|---|---|
| `--volt` | `#FFE600` | Acento amarillo — botones primarios |
| `--blue` | `#1A6FFF` | Azul marca — fondos, bordes |
| `--dark` | `#080C14` | Fondo principal |

---

## Estructura

```
hbelectrics/
├── index.html                     ← Landing principal
├── hbelectrics-coming-soon.html   ← Coming Soon
├── public/                        ← Fotos de proyectos reales
└── favicon.*                      ← Favicons
```

---

## Deploy

Sitio estático — funciona en cualquier hosting:

```bash
# Netlify Drop, GitHub Pages, Vercel, o cualquier servidor nginx/apache
# No requiere build — abrir index.html directamente
```

---

*HBelectrics · Bogotá, Colombia · +57 301 906 2800 · Disponibles 24/7 ⚡*
