# ARQR

El proyecto busca visualizar modelos .glb exportados de Tiltbrush sobre una vista de camara, activando por medio de QRs
Para lograrlo adapté Icosa Gallery-Viewer, diseñado específicamente para ver modelos de Tiltbrush / Openbrush, con extensiones de shaders.

Repo E:/Dev/Projects/gallery-viewer-pats

Edita el index.html y icosa-viewer.module.js en /dist con estas modificaciones:

- Desactiva botón de XR y UI de debugging
- Funcionalidad para cargar modelos de URLs arbitrarios
- Lógica para ajustar posición de camara hardcoded por modelo
- Fondo transparente y vista de camara tras modelo
- Agrega funciones para obtener la posición de la camara

El proyecto esta hosteado en mi github https://github.com/Cdddo/cdddo.github.io/tree/main/ARQR
Los modelos están en repo ARQR https://github.com/Cdddo/ARQR/tree/main/models
Los QRs fueron generados con https://www.qr-code-generator.com

## Known Issues

Hay un problema con los shaders, muestran fondo negro cuando el fondo de la escena es transparente. Intenté pero no pude arreglarlo, creo que es por medio de el shader.