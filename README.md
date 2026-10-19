# FILO — Demostración comercial de Vexel Graphics

Proyecto independiente en español, adaptable a la identidad de cada cliente. HTML, CSS y JavaScript sin dependencias de compilación. Las fotografías fueron generadas para este proyecto. Las marcas y precios son ficticios.

## Organización
- index.html: estructura, marca, textos y navegación.
- style.css: diseño responsive y variables de color.
- app.js: catálogo y comportamiento.
- Imágenes WebP en la raíz: imágenes originales.

## Uso
Abrir index.html para una demostración local o publicar la carpeta del proyecto en un alojamiento estático. El botón de flecha del encabezado abre la administración demo. No tiene contraseña: está pensado para presentaciones, no para datos reales.

## Alcance y límites
Los registros se guardan en localStorage del navegador. No se sincronizan con otros dispositivos. No hay cobros, envío de mensajes, usuarios reales ni conexión con caja o calendario externos. Las recompensas son ilustrativas. Borrar los datos del navegador elimina los registros. No introducir datos personales reales en la demostración.

## Personalizar
Cambiar la marca y textos en index.html; colores en las variables del body; precios, servicios y productos en los arreglos de app.js; reemplazar las imágenes en la raíz manteniendo los nombres. La tipografía usa fuentes del sistema y Georgia, sin dependencias externas.

## Antes de vender como sistema operativo
Conectar base de datos compartida, autenticación del personal, permisos por negocio, validación de precios y disponibilidad en servidor, copias de seguridad y políticas de tratamiento de datos. Configurar cuentas propias para WhatsApp y pagos cuando se contraten. En barbería, resolver las reservas concurrentes con transacciones del servidor; la protección local actual solo sirve para demostración.

## Verificación realizada
Comprobación sintáctica con Node, prueba de cálculo del carrito y filtro de catálogo; prueba de solapamientos, cierre de jornada, bloqueos y liberación de citas canceladas. No se realizó inspección visual con navegador en este entorno.
