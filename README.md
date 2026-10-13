# LandingJJRN

Página creada para la última actividad de Lenguajes de Marcas, a modo de landing page responsive. Evolucionada a portfolio personal de Javier Rodríguez Núñez, con orientación a reporting, datos y CRM.

## Estructura

Se mantiene HTML y CSS, sin frameworks, JavaScript, instalación de dependencias ni compilación:

- `index.html`: presentación, referencia a la imagen original y enlaces principales.
- `Curriculum.html`: currículum organizado en la tabla original.
- `proyectos.html`: tarjetas de proyectos académicos.
- `formulario.html`: formulario y enlaces de contacto.
- `assets/style.css`: estilos agrupados por sección; los ajustes de móvil e impresión están al final.
- `assets/icon.svg`: icono sencillo de la web.
- `assets/img/`: imágenes originales del repositorio, que deben conservarse.

## Aplicar este paquete

Este paquete contiene **solo siete archivos nuevos o modificados**, no una copia completa del repositorio.

1. Copia su contenido sobre tu copia de `LandingJJRN`, conservando las rutas y sustituyendo los archivos correspondientes.
2. **No borres ni reemplaces toda la carpeta `assets`**: combina su contenido y conserva `assets/img` y los demás recursos que ya existen.
3. Abre `index.html` y revisa la web. Después confirma y sube los cambios a GitHub. No subas el ZIP como un archivo: utiliza su contenido.

Se conservan los nombres de las páginas. Respeta la mayúscula inicial de `Curriculum.html` en todos los enlaces.

Para editar el currículum, cambia los textos de `Curriculum.html`; para cambiar colores, usa las variables al principio de `assets/style.css`.

## Menú y móvil

El menú móvil sigue utilizando el checkbox `#ckbox` y CSS. Se abre con clic o con la barra espaciadora cuando el control tiene el foco. No necesita JavaScript. Los enlaces del menú cerrado no se recorren con el teclado.

En móvil, la información de contacto sigue visible y el puesto de trabajo se muestra encima de su descripción. El HTML del currículum sigue siendo una tabla; los roles explícitos conservan la semántica accesible de sus filas y celdas al cambiar su presentación.

## Currículum

Actualización de octubre de 2026, basada en el CV de reporting, datos y CRM: DAM finalizado, separación de las dos etapas de Correos, experiencia anterior en el punto de atención Iberdrola, inglés B2 y preparación de PL-300 **en curso**, no presentada como certificación obtenida. Se distingue el uso profesional de las herramientas de la formación y los proyectos.

Se conserva Museo CMS como proyecto colaborativo, sin presentarlo como desarrollo individual. El correo, GitHub y LinkedIn figuran como vías de contacto. No se añade teléfono ni dirección postal detallada a esta versión pública.

Para imprimir el currículum, utiliza la opción de impresión del navegador: el CSS oculta la navegación y el pie. El documento puede ocupar varias páginas; no se pretende reproducir un PDF de una sola página.

## Formulario: limitación importante

El formulario utiliza `mailto:jjrn87@gmail.com`. El botón **Abrir correo** intenta abrir la aplicación de correo del visitante con los datos del formulario. El visitante debe revisar el mensaje y enviarlo desde esa aplicación.

**No hay servidor de envío, confirmación de entrega ni base de datos.** El comportamiento depende del navegador y del cliente de correo configurado. Se muestra también la dirección para escribir directamente. No se ha añadido un servicio externo de formularios ni se ha enviado ningún correo durante las pruebas.

## Cambios principales

Se conserva la paleta roja y blanca, la portada con dos columnas, las cuatro páginas, la tabla del currículum y las tarjetas. Se han corregido:

- `fomulario_contacto` por `formulario_contacto`, el icono inexistente y las referencias a fuentes que no cargaban. Se usan fuentes del sistema.
- El menú móvil y los estados de foco. Se señala la página activa y se añade un enlace para saltar al contenido.
- Las alturas rígidas y los anchos de los componentes. La información de contacto ya no desaparece en móvil.
- El correo de ejemplo, las etiquetas vacías y los enlaces genéricos a redes sociales.
- Los datos profesionales antiguos y los textos que ofrecían servicios freelance o una respuesta garantizada, que no se corresponden con el enfoque profesional facilitado.

Se ha retirado la dependencia del kit externo de iconos. Las imágenes originales no se sustituyen y no se añaden servicios de terceros.

## Comprobaciones realizadas

Pruebas de renderizado de HTML/CSS en memoria con Chromium, sin navegación por red:

- Las cuatro páginas a 320, 390, 600, 768, 1024 y 1440 píxeles de ancho: sin desbordamiento horizontal en los 24 casos.
- Apertura y cierre del menú con ratón y teclado.
- Visibilidad del contenido de contacto en móvil.
- Campos obligatorios, formato de correo y botón de borrado; sin enviar el formulario.
- Enlace de salto al contenido, destinos internos, IDs y etiquetas de formulario.
- Sintaxis CSS, etiquetas HTML equilibradas, estilos de impresión y preferencia de movimiento reducido.

Limitaciones: no se ha verificado la publicación en GitHub Pages, ni la disponibilidad de todas las demos externas, ni el envío de correos. La imagen original de portada existe en el árbol del repositorio, pero no pudo descargarse al entorno de pruebas; su renderizado no se ha comprobado. No se han realizado pruebas en Safari, Firefox ni móviles físicos. Estas comprobaciones no equivalen a una auditoría completa de accesibilidad.
