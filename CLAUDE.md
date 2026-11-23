# octavioescalante.com — instrucciones para Claude

Web personal de Octavio Escalante, Agente Productor CNV N° 3024. Sitio estático (HTML/CSS, sin build) en Netlify; cada push a `main` se publica solo.

ATENCIÓN: Netlify publica toda la carpeta. Este archivo está bloqueado con `netlify.toml` (devuelve 404). No escribir acá datos personales ni nada que no pueda ser público.

## Estructura
- `index.html` — inicio (estilos inline en `<style>`).
- `guias/` — sección de guías. Estilos compartidos en `guias/guias.css`. Cada guía en `guias/<slug>/index.html` con JSON-LD `Article` + `BreadcrumbList`. Al sumar una guía: tarjeta en `guias/index.html`, entrada en `sitemap.xml` y en `llms.txt`.
- `img/` — logo OE (`oe-logo.png`), logos de Cocos y Balanz en gris.
- `googleb342ad2f5fa22108.html` — verificación de Search Console. No borrar.

## Marca
- Paleta marfil y negro: fondo `#F4F1EA`, papel `#FBF9F5`, tinta `#151515`, texto secundario `#57534C`, acento gris arena `#8C7B5E`, líneas `#DED8CC`.
- Títulos: Cormorant Garamond. Cuerpo: Public Sans.
- Gráficos e ilustraciones: SVG propios, trazo fino (1–1.5 px), sin números de rendimiento.
- Sin fotos de stock ni imágenes generadas por IA de personas.

## Tono
- Español rioplatense, voseo, frases cortas y directas.
- Evitar frases que suenen a IA o a eslogan ("sin vueltas", "a la vista", "desde el primer día", tríadas, "no es X, es Y").
- No nombrar al empleador actual de Octavio.

## Cumplimiento (CNV)
- Nunca prometer ni mostrar rendimientos. Gráficos siempre "ilustrativos".
- Mantener el disclaimer del pie con matrícula AP N° 3024, Cocos Capital S.A. (ALyC N° 688) y Balanz Capital Valores S.A.U. (ALyC Integral N° 210).
- Cambios en textos regulatorios: avisar a Octavio para que los valide con sus ALyC.

## Analítica
- GA4 `G-X07MM6HFDY` en `<head>` de todas las páginas. Toda página nueva lleva el mismo bloque.
- Eventos: `generate_lead` (method: whatsapp / formulario / email), `abrir_cuenta` (broker: cocos / balanz) y `verificar_cnv`.
- Links de apertura: Cocos con link de AP (onelink); Balanz con link genérico sin parámetros de campaña.

## Forma de trabajo
- Mostrar vista previa (capturas) antes de publicar cambios visuales o de texto.
- Commits en español.
