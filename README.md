# Astra Nails — sitio web

Sitio estático de Astra Nails (uñas press-on). Un solo archivo `index.html`
con todo incluido (estilos, JS, imágenes en base64).

## Cómo subirlo a GitHub

### 1. Crear el repositorio
1. Andá a [github.com/new](https://github.com/new)
2. Nombre del repositorio: `astra-nails` (o el que prefieras)
3. Dejalo en **Público** (necesario para GitHub Pages gratis)
4. NO marques "Add a README" (ya tenés uno)
5. Clic en **Create repository**

### 2. Subir los archivos

**Opción fácil (sin terminal):** en la página del repo recién creado, clic en
**"uploading an existing file"**, arrastrá `index.html` y este `README.md`,
y clic en **Commit changes**.

**Opción con terminal**, parado en esta carpeta:
```bash
git init
git add .
git commit -m "Sitio Astra Nails"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/astra-nails.git
git push -u origin main
```
(reemplazá `TU-USUARIO` por tu usuario de GitHub)

### 3. Activar GitHub Pages (para que quede online)
1. En el repositorio, andá a **Settings** (Configuración)
2. En el menú izquierdo, **Pages**
3. En "Source", elegí **Deploy from a branch**
4. Branch: **main**, carpeta: **/ (root)** → **Save**
5. Esperá 1-2 minutos. Wix... digo, GitHub te va a dar una URL tipo:
   `https://TU-USUARIO.github.io/astra-nails/`

Esa es tu página, ya online y gratis.

## Cómo editarlo después

Cualquier cambio de texto, precio o color implica editar el archivo
`index.html` directamente (es HTML/CSS/JS). Podés:
- Editarlo en GitHub mismo: abrí `index.html` en el repo → ícono de lápiz →
  cambiás → **Commit changes** → se actualiza solo en unos minutos
- O pedirme a mí que te genere la versión actualizada y la volvés a subir

## Qué incluye este archivo

- Header con logo (con transparencia) y contacto de Instagram
- Portada con fondo estrellado animado
- Página **Información**: acordeón de FAQ, foto de cómo medir las uñas,
  foto de qué incluye el kit de aplicación
- Página **Diseños**: catálogo de ejemplo con selector de Forma/Largo
- Página **Personalizadas**: formulario de pedido a medida con subida de
  fotos de inspiración (nota: el envío del formulario es solo visual —
  no envía datos a ningún lado todavía, ver abajo)

## Importante: el formulario no envía nada todavía

El formulario de "Personalizadas" está armado visualmente, pero al hacer
clic en "Solicitar cotización" no pasa nada (no te llega ningún correo ni
mensaje). Para que funcione de verdad hay servicios gratuitos como
[Formspree](https://formspree.io) o [Getform](https://getform.io) que se
conectan en unos minutos sin necesitar servidor propio — avisame si querés
que lo dejemos conectado.
