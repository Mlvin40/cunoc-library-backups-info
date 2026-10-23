# NODO App · Información institucional

Sitio estático en español para presentar NODO App y su política de privacidad, con información sobre la integración de respaldos institucionales con Google Drive. HTML5 y CSS3, sin dependencias, JavaScript, formularios ni herramientas de seguimiento.

## Archivos

- `index.html`: presentación institucional.
- `privacy.html`: política de privacidad.
- `styles.css`: diseño compartido, responsive y estilos de impresión.
- `README.md`: documentación y publicación.

Se puede revisar abriendo `index.html` en un navegador. Los enlaces locales son relativos y funcionan también cuando GitHub Pages publica el sitio bajo la ruta de un repositorio.

## Publicación en GitHub Pages

1. Colocar estos cuatro archivos en la raíz del repositorio, en la rama `main`.
2. En GitHub, abrir **Settings → Pages**.
3. En **Build and deployment**, seleccionar **Deploy from a branch**.
4. Elegir la rama **main** y la carpeta **/ (root)**; guardar con **Save**.
5. Esperar la publicación y abrir la dirección que GitHub muestre en esa sección. Comprobar Inicio y Política de privacidad desde esa dirección.

No hace falta compilar ni agregar un workflow al repositorio. GitHub administra el proceso de publicación. La entrega no incluye commits, pushes ni cambios de configuración en GitHub.

Instrucciones oficiales: [Configurar el origen de publicación de GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Antes de publicar y configurar Google OAuth

El sitio está preparado técnicamente para su publicación. Antes de presentarlo como política institucional definitiva, completar o confirmar:

- **Canal oficial de contacto de AEIO CUNOC**, institución responsable del tratamiento, para consultas y solicitudes sobre los datos. Una vez confirmado, incorporarlo en «Consultas y actualizaciones» de `privacy.html`. No se ha inventado un correo ni otro medio de contacto.
- **Funcionamiento real de la integración**: confirmar que el acceso se limita a `drive.file`, que los respaldos se cifran antes de la transferencia y que las finalidades descritas coinciden con la aplicación. No se ha inspeccionado el sistema ni certificado sus medidas de seguridad.
- **Criterios operativos de conservación y eliminación**, quién atiende las solicitudes y cómo se eliminan las copias existentes. Documentarlos cuando estén definidos, sin fijar plazos arbitrarios. Revocar el acceso de Google no borra los respaldos ya guardados.

Una vez publicado, usar la URL real de Inicio y la de `privacy.html` en la configuración de la pantalla de consentimiento de Google OAuth. Mantener coherentes el nombre de la aplicación, el responsable y el contacto. Verificar la titularidad del dominio cuando Google lo solicite. La publicación de estas páginas por sí sola no garantiza la aprobación de Google.

La descripción de `drive.file` sigue la [documentación oficial de Google Drive](https://developers.google.com/workspace/drive/api/guides/api-specific-auth). No es un permiso de acceso general a todo Drive; esta integración declara utilizarlo para los archivos de respaldo que crea.

## Mantenimiento

Actualizar la fecha de revisión en `privacy.html` cuando cambie la política. Mantener el mismo encabezado y pie en ambas páginas. No incorporar credenciales, datos personales, detalles privados de infraestructura ni archivos de respaldo al sitio público.
