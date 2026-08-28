# Descargas Prilso POS

Herramientas de soporte para Prilso POS, de descarga publica.

## PrilsoPOS-Setup.exe

Instalador de la aplicacion completa. Este es un link fijo: cada vez que hay una version nueva se reemplaza este mismo archivo, asi que el link de descarga no cambia -- no hace falta pedir uno nuevo cada vez.

Doble clic, instala en el equipo, crea acceso directo. No requiere permisos de administrador. Abre en una ventana tipo app (sin barra de navegador), sin ventana de consola visible.

Version actual: **1.2.2**

- v1.0.1: incluye la conexion a Supabase (licencias) ya configurada de fabrica.
- v1.0.2: los precios de las cotizaciones ya no suman impuesto encima del precio de Siigo; abre el cajon monedero al cobrar en efectivo; ventana nativa sin consola ni barra de navegador.
- v1.0.3: el campo "Recibido" ya no empieza en 0 (evita que se pegue un cero al escribir); si una cotizacion no logra sincronizar con Siigo, ahora avisa claramente por que en vez de guardar en silencio con el numero local.
- v1.0.4: icono de la pestana/ventana con el logo real (la P) y titulo "PrilsoTech Pos" en vez del generico anterior.
- v1.1.0: descuentos por producto al cobrar, devoluciones/reembolsos (desde Documentos), stock por bodega (Stock > Bodegas), cierre de caja formal con conteo fisico e impresion (Caja > Cerrar caja), y desplegable de usuarios en el login.
- v1.2.0: pantalla de "Configuracion inicial" ampliada (datos de la empresa y, si ya los tienes, credenciales de Siigo, todo en un solo paso); permisos por usuario mas completos.
- v1.2.1: la sincronizacion con Siigo ya no sobreescribe el inventario local (las cotizaciones no descuentan stock en Siigo, asi que ese numero ya no se le impone a Prilso); la cotizacion impresa/PDF ya no muestra desglose de IVA, solo cantidad, precio unitario, total, descuento y total a pagar.
- v1.2.2: la app ya puede buscar y aplicar actualizaciones desde adentro (Admin > Licencia > "Actualizar ahora") -- descarga el instalador de este mismo link y lo abre, sin tener que venir aqui a buscarlo a mano. Si el equipo bloquea abrir el instalador por politicas de seguridad, se ve un aviso con este mismo link para descargarlo manual.

## ResetAdminPin.exe

Restablece el PIN del administrador (o de cualquier usuario) directo en la base de datos local, para cuando se pierde el acceso. No necesita Python instalado.

**Uso:**
1. Cierra el servidor de Prilso POS en ese equipo si esta corriendo.
2. Doble clic en `ResetAdminPin.exe`.
3. Busca la base de datos sola; si no la encuentra, pide la ruta completa.
4. Pide el usuario a restablecer (Enter = admin).
5. Muestra un PIN nuevo en pantalla -- anotalo, no se vuelve a mostrar.
6. Abre Prilso POS y entra con ese usuario y el PIN nuevo.
