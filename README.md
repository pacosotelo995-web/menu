# San Judas Tadeo · Menú del Food Truck

Página web del menú del food truck **San Judas Tadeo** (Familia Sotelo), comida mexicana en Chicago.

Es un sitio **estático**: solo HTML y CSS. No tiene servidor, base de datos, formularios ni JavaScript, así que no guarda datos de nadie.

## Archivos

| Archivo | Para qué sirve |
|---|---|
| `index.html` | El menú |
| `styles.css` | Colores, letras y diseño |
| `404.html` | Página que sale cuando un enlace no existe |
| `favicon.svg`, `favicon.png` | Iconito de la pestaña del navegador |
| `og-image.png` | Imagen que sale al compartir el enlace en Facebook, WhatsApp, etc. |
| `robots.txt` | Permite que Google encuentre la página |

## Verlo en tu computadora

Abre `index.html` con doble clic, o sirve la carpeta con cualquier servidor local:

```bash
npx serve .
```

## Cambiar precios o platillos

1. Abre `index.html` con un editor de texto.
2. Busca el platillo y cambia el nombre, la descripción o el precio.
3. Guarda, haz commit y push. Render publica el cambio solo, en uno o dos minutos.

## Publicación (Render)

- Tipo: **Static Site**
- Rama: `main`
- Build command: *(vacío)*
- Publish directory: `.`
- Encabezados de seguridad configurados en Render: Content-Security-Policy, Strict-Transport-Security, X-Frame-Options, X-Content-Type-Options, Referrer-Policy y Permissions-Policy.

## Seguridad

- No hay claves ni contraseñas en el código. Si algún día se agregan, van en variables de entorno de Render o en un archivo `.env`, que está en `.gitignore`.
- La página tiene una Content Security Policy que solo permite cargar estilos propios y las fuentes de Google Fonts.
- Render da HTTPS automático.
- Errores y registros: Render guarda los registros de cada publicación en su panel.
