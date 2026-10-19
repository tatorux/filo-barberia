# FILO Studio · Aplicación de reservas v2

Demostración comercial por Vexel Graphics. Experiencia de studio y agenda con identidad en lavanda, ciruela, negro y salvia. El recorrido y el diseño son independientes de BRASA.

**Página:** https://tatorux.github.io/filo-barberia/

## Recorridos
- Studio: servicios, equipo, próxima cita y tarjeta de miembro.
- Reserva en 4 pasos: ritual, profesional, fecha/hora y confirmación.
- Disponibilidad en intervalos de 15 minutos, duración de servicio y 10 minutos entre citas.
- Horario: lunes a sábado, 09:00–19:00, zona America/Bogota; máximo 30 días por adelantado.
- Mis citas: próximas e historial, detalle, reprogramación y cancelación confirmada.
- Inspiración: looks y acceso directo al servicio asociado.
- Mi espacio: perfil y exportación/importación de respaldo JSON.
- Administración `#admin`: agenda por día/profesional, estados y bloqueo de jornadas. No se permite bloquear una jornada con citas confirmadas, ni reactivar reservas que chocan con otra cita.

## Archivos
`index.html`, `style.css`, `app.js`: entrada, diseño y comportamiento. `icon.svg`, `app.webmanifest` y fotografías WebP. Aplicación sin compilación, publicable en GitHub Pages. El manifiesto declara visualización standalone en navegadores compatibles; no se promete funcionamiento offline.

## Personalización
Cambiar `services`, `team`, constante `BUFFER` y reglas de `canBook()` en app.js. Colores en `:root` de style.css. Todos los nombres, marcas y tarifas son ficticios; las fotografías son generadas para la demo.

## Datos y límites
Almacena reservas bajo `filo-v2` en `localStorage`. Sin autenticación, sincronización entre dispositivos, agenda real, mensajes, cobros o integraciones. No introducir datos personales reales. La disponibilidad evita cruces en el estado local; no puede garantizar exclusión entre clientes simultáneos sin un servidor.

La versión inicial usaba `filo-bookings`; sus registros no se migran porque el modelo cambió. En v2 el historial comienza vacío.

El programa de miembro cuenta servicios marcados “Completada”. Cada cinco muestra un beneficio ilustrativo que se gestionaría con el negocio; no aplica automáticamente un servicio gratuito ni tiene valor real.

## Para producción
Base de datos y reservas transaccionales, autenticación y permisos, verificación de cliente, disponibilidad autoritativa en servidor, políticas de cancelación, protección de datos y recordatorios con proveedores propios. La administración local abierta es únicamente demostrativa.

## Validación v2
Node: sintaxis, rangos de horarios, domingos, cierre, margen de preparación, solapamientos, independencia entre profesionales, reprogramación, liberación al cancelar, bloqueos y renderizado de los cuatro pasos. Inspección final en navegador de Pages. Las reglas responsive no sustituyen pruebas en todos los dispositivos físicos.
