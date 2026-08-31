# Descargas Prilso POS

Herramientas de soporte para Prilso POS, de descarga publica.

## PrilsoPOS-Setup.exe

Instalador de la aplicacion completa. Este es un link fijo: cada vez que hay una version nueva se reemplaza este mismo archivo, asi que el link de descarga no cambia -- no hace falta pedir uno nuevo cada vez.

Doble clic, instala en el equipo, crea acceso directo. No requiere permisos de administrador. Abre en una ventana tipo app (sin barra de navegador), sin ventana de consola visible.

Version actual: **1.0.0**

Version completa reiniciada desde cero: Cotizacion 100% local (nunca toca Siigo), Factura real de Siigo con envio automatico a la DIAN en el mismo paso, licencia y sesion de Siigo marcadas en verde cuando ya estan activas, boton de salida con opciones de cerrar sesion / salir del programa / apagar el equipo, y varias correcciones de estabilidad acumuladas.

## ResetAdminPin.exe

Restablece el PIN del administrador (o de cualquier usuario) directo en la base de datos local, para cuando se pierde el acceso. No necesita Python instalado.

**Uso:**
1. Cierra el servidor de Prilso POS en ese equipo si esta corriendo.
2. Doble clic en `ResetAdminPin.exe`.
3. Busca la base de datos sola; si no la encuentra, pide la ruta completa.
4. Pide el usuario a restablecer (Enter = admin).
5. Muestra un PIN nuevo en pantalla -- anotalo, no se vuelve a mostrar.
6. Abre Prilso POS y entra con ese usuario y el PIN nuevo.
