# COMUNICA · Comunicación para secundaria

Página web estática compatible con GitHub Pages. Incluye portada, entrada de estudiante, lecturas aleatorias y subrayado con cursor, lápiz, paleta y borrador. La versión publicada únicamente con GitHub Pages funciona en **modo demostración**: **no centraliza ni guarda nombres completos de estudiantes**, y el panel docente requiere un servidor adicional. No publicar ninguna base de datos, contraseña, CSV de alumnado o carpeta `data/` en este repositorio público.

## Crear la web pública con GitHub Pages

1. En la cuenta GitHub `miguelpinto9988-byte`, crea un repositorio público llamado `miguelpinto9988-byte.github.io` para tener una web en la dirección `https://miguelpinto9988-byte.github.io/`.
2. Sube `index.html` y `.nojekyll` a la raíz de la rama `main`.
3. En `Settings > Pages`, configura `Build and deployment > Deploy from a branch`, rama `main`, carpeta `/ (root)`, y guarda.
4. Confirma que GitHub muestra la dirección pública de Pages. El despliegue puede tardar.

## Dominio propio

Cuando tengas un dominio registrado, ve a `Settings > Pages > Custom domain`, escribe **tu dominio real** y guárdalo. En el panel DNS del registrador configura los registros adecuados según sea un subdominio (CNAME) o dominio raíz (A/AAAA/ALIAS), siguiendo la documentación oficial. Verifica el dominio y activa `Enforce HTTPS` cuando esté disponible. No escribas un dominio de ejemplo en el archivo `CNAME`.

Documentación oficial: https://docs.github.com/es/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site

## Registros de estudiantes y panel docente

GitHub Pages no ejecuta Python ni SQLite y por sí solo no puede centralizar registros desde distintos equipos. Para esta función, se requiere alojar el servidor `app.py` de la versión completa en un servicio compatible con Python, con HTTPS y datos persistentes. El propio panel docente necesita autenticación activa en ese servidor. Hasta que esté conectado, **no uses esta demostración para recoger nombres reales de alumnos**.

Se deben obtener las autorizaciones pertinentes del centro educativo y respetar la normativa de protección de datos aplicable antes de recopilar información de menores.