# CLAUDE.md — Proyecto HBelectrics
> Guía maestra del proyecto de identidad digital y landing page para **HBelectrics**, empresa de servicios eléctricos en Bogotá y alrededores.

---

## 📋 ÍNDICE DE TAREAS

| # | Tarea | Estado | Archivo |
|---|-------|--------|---------|
| 01 | Página "Próximamente" (Coming Soon) | ⬜ Pendiente | `hbelectrics-coming-soon.html` |
| 02 | Landing Page principal de ventas | ✅ Completada | `electricistas-bogota-landing.html` |
| 03 | Galería de trabajos + Sección de videos | ✅ Completada | (integrada en landing) |
| 04 | Paleta de colores de marca aplicada | ✅ Completada | (integrada en landing) |
| 05 | Formulario de cotización → WhatsApp | ✅ Completada | (integrada en landing) |

---

## 🏢 INFORMACIÓN DE LA EMPRESA

```
Nombre:        HBelectrics
Servicio:      Electricistas a domicilio — hogares, negocios, industrias
Ciudad:        Bogotá D.C. y alrededores (municipios cercanos)
Teléfono:      +57 301 906 2800
WhatsApp:      https://wa.me/573019062800
Disponibilidad: 24/7 incluyendo festivos
```

---

## 🎨 IDENTIDAD DE MARCA

### Colores oficiales
| Variable CSS | Hex | Uso |
|---|---|---|
| `--volt` | `#FFE600` | Acento amarillo — botones primarios, stats, estrellas |
| `--volt-dim` | `#c9b700` | Amarillo oscuro — hovers |
| `--blue` | `#1A6FFF` | Azul marca — botones nav, fondos, bordes activos |
| `--blue-dim` | `#1458cc` | Azul oscuro — gradientes |
| `--blue-light` | `#4D90FF` | Azul claro — textos, badges, íconos |
| `--dark` | `#080C14` | Fondo principal |
| `--dark2` | `#0D1420` | Fondo secciones alternas |
| `--dark3` | `#121B2E` | Cards, formularios |
| `--gray` | `#7A8899` | Textos secundarios |
| `--white` | `#ffffff` | Textos principales |

### Tipografías
| Tipo | Fuente | Uso |
|---|---|---|
| Display / Títulos | `Bebas Neue` | Headings H1–H3, estadísticas, sección tags |
| Cuerpo / UI | `Nunito` | Párrafos, botones, labels, formularios |

### Identidad visual del logo
- El logo combina **amarillo** (`--volt`) + **azul** (`--blue`)
- En navegación: `⚡` (rayo amarillo) + `HB` (azul claro) + `electrics` (amarillo)
- Siempre usar fondo oscuro bajo el logo

### Tono de comunicación
- Directo, confiable, urgente pero profesional
- Verbos de acción: "Llamar Ahora", "Solicitar", "Resolver"
- Énfasis en: **velocidad** (60 min), **garantía escrita**, **precio justo**, **24/7**
- Nunca usar lenguaje pasivo o técnico sin explicación

---

## 🗂️ ESTRUCTURA DE ARCHIVOS DEL PROYECTO

```
hbelectrics/
├── CLAUDE.md                          ← Este archivo
├── hbelectrics-coming-soon.html       ← TAREA 01 (por crear)
└── electricistas-bogota-landing.html  ← Landing principal (completa)
```

---

## ✅ TAREA 01 — PÁGINA "PRÓXIMAMENTE" (COMING SOON)

### Descripción
Crear una página de **"Próximamente"** elegante y profesional que se mostrará mientras el sitio web definitivo de HBelectrics está en construcción. Debe generar expectativa, transmitir confianza desde el primer momento y capturar leads.

### Referencia de concepto
Similar a la página de **Thisa**:
```
Thisa
Próximamente
Estamos construyendo algo especial
Software a la medida para PYMEs y Emprendimientos en Colombia
```
Adaptar ese concepto minimalista y elegante para HBelectrics.

### Requisitos de contenido
- [ ] Logo/nombre `HBelectrics` con rayo ⚡
- [ ] Headline: algo como *"Algo poderoso está por llegar"* o *"Tu electricista de confianza, ahora en línea"*
- [ ] Subtítulo breve que explique el servicio
- [ ] **Contador regresivo** (fecha objetivo: configurable, ej. 30 días desde hoy)
- [ ] **Formulario de captura de leads** — nombre + teléfono/WhatsApp → botón "Avisarme cuando esté listo"
- [ ] **Botón de contacto directo** — "¿Necesitas un electricista ya? Llámanos" → `tel:3019062800`
- [ ] **Botón WhatsApp** flotante o prominente
- [ ] Redes sociales (placeholders si no se tienen aún)
- [ ] Frase de confianza: *"Más de 800 clientes atendidos en Bogotá"*

### Requisitos de diseño
- Fondo oscuro azul noche (`#080C14` a `#0D1420`) con efecto de partículas o grid sutil
- Acento amarillo `#FFE600` + azul `#1A6FFF` — coherente con la landing principal
- Tipografías: `Bebas Neue` (títulos) + `Nunito` (cuerpo) — igual que la landing
- Animaciones: entrada suave (fade-up staggered), contador animado, partículas de fondo opcionales
- Rayo ⚡ animado o con efecto glow pulsante en el hero
- 100% responsive — mobile first
- Sin dependencias externas excepto Google Fonts

### Requisitos técnicos
- Archivo único HTML (sin frameworks)
- El formulario de "Avisarme" debe enviar los datos a WhatsApp: `https://wa.me/573019062800`
- Contador regresivo en JavaScript puro — fecha configurable al inicio del script
- Meta tags SEO básicos: title, description, og:title, og:description
- Favicons placeholder con emoji ⚡

### Estructura de secciones (de arriba a abajo)
```
1. HERO FULL SCREEN
   └── Logo HBelectrics + tagline + countdown + CTA principal

2. MINI BARRA DE CONFIANZA (opcional, justo debajo del fold)
   └── ⚡ 24/7  |  🛡️ Garantía escrita  |  📍 Bogotá y alrededores

3. FORMULARIO DE NOTIFICACIÓN
   └── "Sé el primero en saberlo" + input nombre + input teléfono + botón

4. CONTACTO DIRECTO
   └── "¿Emergencia ahora? No esperes al lanzamiento."
       Botón llamar + Botón WhatsApp

5. FOOTER MINIMAL
   └── © 2025 HBelectrics · +57 301 906 2800
```

### Nombre del archivo de salida
```
hbelectrics-coming-soon.html
```

---

## ✅ TAREA 02 — LANDING PAGE PRINCIPAL (COMPLETADA)

### Descripción
Landing page completa de alta conversión para HBelectrics. Incluye:

- Hero con formulario de cotización integrado que envía a WhatsApp
- Barra de trust (certificaciones, garantía, tiempo respuesta)
- Sección de servicios (6 cards: cortos, sin energía, instalaciones, cableado, consumo, industrial)
- Sección "Por qué elegirnos" con 3 diferenciadores + visual de stats
- **Galería de trabajos** — grid masonry 2 filas, 6 fotos, hover con overlay
- **Sección de videos** — video principal + 3 videos secundarios en panel lateral
- Testimonios (3 reseñas de clientes)
- Banner de emergencia CTA
- Footer completo con zonas y servicios
- Botón WhatsApp flotante con animación pulsante

### CTAs principales (todos conectados al número real)
```
Llamar:     tel:3019062800
WhatsApp:   https://wa.me/573019062800
```

### Cómo personalizar la galería
En el archivo `electricistas-bogota-landing.html`, buscar las etiquetas `<img>` dentro de `.gitem` y reemplazar las URLs de Unsplash por las rutas de las fotos reales:
```html
<!-- ANTES (foto de referencia) -->
<img src="https://images.unsplash.com/photo-XXXX?w=800&q=80" alt="..."/>

<!-- DESPUÉS (foto real) -->
<img src="./fotos/tablero-chapinero.jpg" alt="Instalación tablero Chapinero"/>
```

### Cómo agregar video de YouTube
En el script al final del archivo, buscar:
```javascript
const VIDEO_ID = 'TU_VIDEO_ID';
```
Reemplazar `TU_VIDEO_ID` por el ID del video de YouTube. Ejemplo:
- URL del video: `https://www.youtube.com/watch?v=ABC123xyz`
- ID del video: `ABC123xyz`
- Resultado: `const VIDEO_ID = 'ABC123xyz';`

---

## 🔧 ESTÁNDARES TÉCNICOS DEL PROYECTO

### Stack tecnológico
- **HTML5** semántico
- **CSS3** con variables CSS (sin preprocesadores)
- **JavaScript vanilla** (sin jQuery ni frameworks)
- **Google Fonts** vía CDN (Bebas Neue + Nunito)
- Sin WordPress, sin Elementor, sin dependencias pesadas

### Patrones de código establecidos
```css
/* Variables siempre en :root */
:root {
  --volt: #FFE600;
  --blue: #1A6FFF;
  --blue-light: #4D90FF;
  --dark: #080C14;
  /* etc... */
}

/* Botón primario — amarillo */
.btn-primary {
  background: var(--volt);
  color: var(--dark);
  border-radius: 50px;
  font-weight: 800;
}

/* Botón secundario — azul */
.btn-blue {
  background: var(--blue);
  color: var(--white);
  border-radius: 50px;
}
```

### Patrón de animaciones
```css
/* Entrada de elementos al hacer scroll */
.reveal {
  opacity: 0;
  transform: translateY(40px);
  transition: opacity .7s ease, transform .7s ease;
}
.reveal.visible {
  opacity: 1;
  transform: translateY(0);
}
```
```javascript
// IntersectionObserver para activar .reveal
const obs = new IntersectionObserver((entries) => {
  entries.forEach((e, i) => {
    if (e.isIntersecting) {
      e.target.style.transitionDelay = (i % 4) * 0.08 + 's';
      e.target.classList.add('visible');
    }
  });
}, { threshold: 0.1 });
document.querySelectorAll('.reveal').forEach(el => obs.observe(el));
```

### Patrón de envío a WhatsApp
```javascript
function sendWA() {
  const name    = document.querySelectorAll('input')[0].value || 'Sin nombre';
  const phone   = document.querySelectorAll('input')[1].value || 'Sin teléfono';
  const service = document.querySelector('select').value     || 'No especificado';
  const address = document.querySelectorAll('input')[2].value|| 'Sin dirección';
  const msg = `Hola HBelectrics! Necesito una cotización:\n\n👤 Nombre: ${name}\n📞 Teléfono: ${phone}\n⚡ Servicio: ${service}\n📍 Dirección: ${address}`;
  window.open('https://wa.me/573019062800?text=' + encodeURIComponent(msg), '_blank');
}
```

### Responsive breakpoints
```css
@media (max-width: 900px) { /* Tablet */ }
@media (max-width: 600px) { /* Móvil */ }
```

---

## 📱 INFORMACIÓN DE CONTACTO OFICIAL

> ⚠️ Usar estos datos en **TODOS** los archivos del proyecto. No inventar ni cambiar.

```
Empresa:     HBelectrics
Teléfono:    3019062800
WhatsApp:    +57 301 906 2800
WA URL:      https://wa.me/573019062800
Call URL:    tel:3019062800
Cobertura:   Bogotá y alrededores (toda la ciudad + municipios)
Horario:     24/7 incluyendo festivos y fines de semana
```

---

## 🚀 PRÓXIMAS TAREAS SUGERIDAS (BACKLOG)

| # | Tarea | Prioridad |
|---|-------|-----------|
| 06 | Página de servicios detallados (cada servicio con su propia sección) | Alta |
| 07 | Sección "Antes y Después" de trabajos reales | Alta |
| 08 | Integración con Google Reviews (widget embed) | Media |
| 09 | Blog/artículos SEO: "Qué hacer en un corto circuito en Bogotá" | Media |
| 10 | Página de confirmación post-formulario ("Gracias, te contactamos pronto") | Baja |
| 11 | Versión dark/light toggle | Baja |
| 12 | Chat en vivo integrado (Tawk.to u otro gratuito) | Media |

---

## 📝 NOTAS IMPORTANTES PARA CLAUDE

1. **Siempre mantener coherencia** con la paleta azul + amarillo sobre fondo oscuro
2. **Nunca usar Inter, Roboto o Arial** — usar Bebas Neue + Nunito
3. **Todos los botones de acción** deben conectar con `tel:3019062800` o `https://wa.me/573019062800`
4. **El diseño es dark-first** — fondo oscuro, no blanco
5. **Cero dependencias de WordPress** — todo HTML/CSS/JS puro
6. Al crear nuevas páginas, **importar Google Fonts** así:
   ```html
   <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Nunito:wght@400;600;700;800&display=swap" rel="stylesheet"/>
   ```
7. Cada nueva página debe ser **un archivo HTML único** — sin archivos CSS o JS separados
8. Las fotos de Unsplash son **placeholders temporales** — deben reemplazarse con fotos reales de HBelectrics

---

*Última actualización: Marzo 2025 · HBelectrics · Bogotá, Colombia ⚡*
