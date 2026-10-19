MI INVENTARIO — VERSIÓN 1.2.0 DE PRUEBAS
======================================

ATENCIÓN: Este paquete contiene SOLO el código de la aplicación.
No contiene las láminas, imágenes ni stock almacenados en la tablet del cliente.
NO reemplaces los archivos de la instalación original hasta recuperar y
comprobar una copia de seguridad actual y hacer la prueba de migración.

CAMBIOS EN ESTA VERSIÓN
----------------------
1. Al tocar una foto se abre a pantalla completa; botón X para cerrar.
2. En Administrador > Editar lámina se puede rotar la imagen 90° a izquierda/derecha.
   La imagen original se conserva sin editar y el giro se guarda en el producto.
3. Las tarjetas del Dashboard de stock bajo/sin stock abren un informe por carpeta.
4. Las láminas aparecen por orden de ingreso y se pueden reordenar arrastrando
   el controlador ☰ Mover lámina (solo administrador).
5. Nuevo respaldo ZIP por partes, con imágenes binarias, sin Base64 gigante.
6. Configuración > Comprobar ZIP descargado: valida todas las partes y los
   checksums de las imágenes sin restaurar ni modificar el inventario.
7. Modo cliente: muestra automáticamente TODAS las carpetas creadas; el cliente
   puede entrar, volver y elegir otra carpeta sin entrar en Configuración.
   El modo cliente no muestra controles de editar, crear, eliminar ni cambiar stock.
   Se eliminó la antigua selección "Carpeta visible para el cliente".
   "Iniciar automáticamente en modo cliente" funciona sin asignar una carpeta.

RESPALDOS Y RESTAURACIÓN
-----------------------
- Entra como administrador, abre Configuración y elige "Crear copia de seguridad
  ZIP por partes". Descarga las partes una a una y verifica que cada archivo
  esté guardado en Descargas. El número de partes depende del tamaño de imágenes.
- Conserva TODAS las partes ZIP juntas, junto a una copia adicional fuera
  de la tablet (PC/USB/nube).
- Para comprobar un respaldo sin cambiar los datos, usa "Comprobar ZIP descargado"
  y selecciona TODOS sus archivos ZIP al mismo tiempo. Comprueba el resultado.
- "Restaurar copia de seguridad" REEMPLAZA todos los datos actuales. Úsalo
  primero en una instalación y un origen de almacenamiento INDEPENDIENTES.
- También se pueden restaurar respaldos antiguos JSON (solo para pruebas).

INSTALACIÓN / ACTUALIZACIÓN
--------------------------
Mantén la estructura de archivos HTML, CSS y JavaScript de esta carpeta.
Los datos de la aplicación se guardan en IndexedDB del navegador/instalación,
NO dentro de los archivos HTML/JS de este paquete.

ADVERTENCIA DE SEGURIDAD IMPORTANTE
----------------------------------
La información local depende del navegador y del origen (dominio/ruta) de la
aplicación. Un cambio de URL, cambio de perfil, "Borrar datos del sitio" o
reinstalación puede dejar de mostrar los datos de la tablet aunque los archivos
HTML/JS sean iguales. El ZIP NO copia los datos actuales del cliente.
La contraseña controla la interfaz, no es autenticación de un servidor.

ANTES DE PASAR A PRODUCCIÓN
--------------------------
1. Conseguir una copia ACTUAL del cliente y verificarla.
2. Restaurarla en una instalación de pruebas y comprobar cantidades y fotos.
3. Probar la aplicación en la tablet Android real con ese respaldo.
4. Solo entonces planificar el reemplazo de código conservando el mismo origen,
   almacenamiento y navegador, con plan para volver atrás.

Contraseña original (solo instalaciones nuevas): 1234. Cambiarla en Ajustes.
