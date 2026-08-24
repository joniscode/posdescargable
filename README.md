# Descargas Prilso POS

Herramientas de soporte para Prilso POS, de descarga publica.

## PrilsoPOS-Setup-1.0.1.exe

Instalador de la aplicacion completa. Doble clic, instala en el equipo, crea acceso directo. No requiere permisos de administrador.

v1.0.1: incluye la conexion a Supabase (licencias) ya configurada de fabrica -- antes de esta version la activacion de licencia no podia funcionar en un equipo instalado.

## ResetAdminPin.exe

Restablece el PIN del administrador (o de cualquier usuario) directo en la base de datos local, para cuando se pierde el acceso. No necesita Python instalado.

**Uso:**
1. Cierra el servidor de Prilso POS en ese equipo si esta corriendo.
2. Doble clic en `ResetAdminPin.exe`.
3. Busca la base de datos sola; si no la encuentra, pide la ruta completa.
4. Pide el usuario a restablecer (Enter = admin).
5. Muestra un PIN nuevo en pantalla -- anotalo, no se vuelve a mostrar.
6. Abre Prilso POS y entra con ese usuario y el PIN nuevo.
