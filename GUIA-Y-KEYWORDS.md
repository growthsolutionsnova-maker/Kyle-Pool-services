# Coughlin Pool Service — Guía rápida del sitio web

## 1. Qué hay en esta carpeta

| Archivo | Para qué sirve |
|---|---|
| `index.html` | El sitio completo, con textos, estilos y funciones. |
| `assets/` | Las fotos, los logos y el mapa. |
| `fonts/` | Las tipografías. |
| `og-image.jpg` | La imagen que aparece al compartir el enlace por WhatsApp o Facebook. |
| `logo.png` | El logo que usa Google. |
| `sitemap.xml` / `robots.txt` | Archivos para que Google encuentre el sitio. |
| `favicon.ico` | El ícono de la pestaña del navegador. |

> También tienes **`index-single-file.html`**. Es el sitio en **un solo archivo** con todo incluido, y funciona sin internet. Sirve para mostrarlo o guardarlo. **Para publicarlo usa esta carpeta**, que carga mucho más rápido: saca 96/100 en velocidad, contra 61/100 del archivo único.

---

## 2. Publicar gratis en GitHub Pages

1. Crea una cuenta en **github.com**.
2. Crea un repositorio nuevo, por ejemplo `coughlinpoolservice`, y márcalo como **Public**.
3. Pulsa **"uploading an existing file"** y arrastra **todo el contenido de esta carpeta** (index.html, assets, fonts, etc.).
4. Ve a **Settings → Pages → Branch: main → Save**.
5. En 1 o 2 minutos el sitio estará en `https://TU-USUARIO.github.io/coughlinpoolservice/`.

**Si tienes dominio propio**, en Settings → Pages → Custom domain escribe `www.tudominio.com` y configura el DNS como indica GitHub.

---

## 3. Cambiar el dominio en el código (importante)

El sitio usa `https://growthsolutionsnova-maker.github.io/Kyle-Pool-services` como dirección provisional. Cuando sepas tu dirección final, abre estos archivos con un editor de texto (TextEdit en Mac, o VS Code) y usa **Buscar y reemplazar**:

- `index.html`
- `sitemap.xml`
- `robots.txt`

Busca `https://growthsolutionsnova-maker.github.io/Kyle-Pool-services` y reemplázalo por tu dirección real, sin barra al final.

---

## 4. Cambios comunes (en `index.html`)

Usa **Buscar y reemplazar en todo el archivo**.

### Teléfono / WhatsApp
El número aparece en tres formatos. Cambia los tres:
- `(561) 305-9345` es el texto visible.
- `+15613059345` es el enlace para llamar (`tel:`).
- `15613059345` es el enlace de WhatsApp (`wa.me/`).

Busca también `+1-561-305-9345`, que está en los datos para Google.

### Horario
Busca `7 AM – 7 PM`, `7:00 AM – 7:00 PM` y `"opens": "07:00"` / `"closes": "19:00"`.

### Textos
- **Inglés:** está en el HTML. Busca la frase y cámbiala.
- **Español y portugués:** están al final del archivo, dentro de `window.CPS_I18N = { es:{…}, pt:{…} }`. Cada texto tiene una clave igual a la del inglés; por ejemplo, `"hero.h1a":"Piscinas Cristalinas."`.
- Si cambias una frase en inglés, cambia también su versión en `es` y `pt`.

### Fotos
Reemplaza el archivo en `assets/` por uno nuevo **con el mismo nombre**:

| Archivo | Dónde aparece |
|---|---|
| `hero.webp` (1600 px) y `hero-800.webp` (800 px) | Portada |
| `weekly.webp` | Weekly Pool Service |
| `repairs.webp` | Pool Repairs |
| `chemistry.webp` | Water Chemistry |
| `green-split.webp` | Tarjeta Green-to-Clean |
| `before.webp` / `after.webp` | Deslizador antes y después |

Consejo: usa formato **WebP**, de menos de 150 KB. Puedes convertir fotos gratis en squoosh.app.

### Reseñas de Google ⚠️ (pendiente)
Busca `PASTE REAL GOOGLE REVIEW`. Hay 4 tarjetas; en cada una cambia:
- el texto entre `<blockquote>` y `</blockquote>`,
- la letra del avatar (`rv__avatar`),
- `[Customer Name]`, `[City]` y `[Month Year]`.

**Nunca publiques reseñas inventadas.** Además, las reglas de la FTC en EE. UU. lo prohíben.

Busca también `[GOOGLE-REVIEW-LINK]` y pon el enlace de tu perfil de Google Business.

### Redes sociales (pendiente)
Busca `SOCIAL:` en el footer. Quita los símbolos `<!--` y `-->` y pon tus enlaces de Instagram o Facebook.

### Foto del dueño (opcional)
Busca `OWNER PHOTO`. Ahí va tu foto, que genera mucha confianza.

---

## 5. Palabras clave SEO usadas

Están en el título, la descripción, los textos y los datos para Google:

1. pool service Boca Raton
2. pool cleaning Boca Raton
3. weekly pool service Boca Raton
4. pool repair Boca Raton
5. pool maintenance Delray Beach
6. pool service Deerfield Beach
7. pool cleaning Boynton Beach
8. pool service Parkland FL
9. pool service Coconut Creek
10. pool service Lighthouse Point
11. pool service Lake Worth
12. pool pump repair Boca Raton
13. pool heater repair Palm Beach County
14. green pool cleanup Boca Raton
15. pool service near me

**Siguiente paso recomendado para SEO:** crea o completa tu perfil de **Google Business Profile** con el mismo nombre, teléfono y ciudades del sitio. Es lo que más te hará aparecer en "pool service near me".

---

## 6. Resultados de la revisión final

| Prueba | Resultado |
|---|---|
| Lighthouse, versión para publicar (celular) | Rendimiento 96 · Accesibilidad 100 · Buenas prácticas 100 · SEO 100 |
| Datos para Google (JSON-LD) | Válidos: negocio local, 4 servicios, 10 preguntas y ruta de navegación |
| Imágenes con carga diferida | 9 de 12. La foto de portada y los 2 logos del menú cargan al instante. |
| Idiomas | EN, ES y PT funcionan, incluidos el formulario y el mensaje de WhatsApp |
| Pantallas probadas | 320, 360, 375, 480, 768, 1024, 1440 y 1920 px, sin desbordes laterales |
| Sin JavaScript | Todo el contenido se ve |
| Errores de consola | 0 |
| Tamaño | Carpeta para publicar: 1,3 MB en total; el HTML pesa 142 KB. Archivo único: 1,5 MB. |

**Formulario:** envía los datos por **WhatsApp o SMS** al (561) 305-9345. No usa Formspree porque el negocio no tiene correo. Si más adelante creas uno, se puede conectar.
