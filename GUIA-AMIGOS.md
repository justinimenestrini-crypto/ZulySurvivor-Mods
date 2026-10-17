# ModsEx — Juega en ZulySurvivor

## Descargar

[Descargar ModsEx Setup 1.4.2 para Windows de 64 bits](https://github.com/justinimenestrini-crypto/ZulySurvivor-Mods/releases/download/v1.4.2/ModsEx-Setup-1.4.2-x64.exe)

[Ver todas las descargas](https://github.com/justinimenestrini-crypto/ZulySurvivor-Mods/releases/latest)

Usa Setup para recibir actualizaciones desde el programa. El portable se actualiza manualmente. No necesitas cuenta ni token de GitHub para descargar o sincronizar mods.

## Primera instalación

1. Instala ModsEx ejecutando Setup.
2. Prepara un perfil de Minecraft Java **1.21.11 con Forge** en tu launcher de Minecraft. Minecraft requiere Java 21 para esta versión. ModsEx gestiona mods; no instala Minecraft, Forge ni Java y no inicia el juego.
3. Abre la carpeta del perfil con el que jugarás. En ModsEx → Configuración → Elegir carpeta selecciona su carpeta `mods` y guarda. Si usas TLauncher con una carpeta de versión independiente, selecciona esa carpeta, no la de otro perfil.
4. Conserva esta URL del catálogo: `https://raw.githubusercontent.com/justinimenestrini-crypto/ZulySurvivor-Mods/main/mods.json`.
5. Con Minecraft cerrado, entra en Mi colección → Comprobar → Instalar faltantes.
6. Abre Minecraft con el perfil Forge 1.21.11. Comprueba en el botón Mods que los archivos se cargaron.
7. En Multijugador añade `ZulySurvivor.aternos.me`. El servidor debe estar encendido para entrar.

Usa una carpeta de perfil independiente. Los mods de otras versiones que ya tengas no se retiran automáticamente. Si instalaste `afterburner-0.1.27.jar` con Forge 61.1.5, retíralo desde Mods locales: exige Forge 61.2 o posterior y ya no forma parte del catálogo compartido.

## Actualizar

- Nuevos mods: Mi colección → Comprobar → Instalar faltantes. No hace falta descargar el launcher de nuevo.
- Nuevo programa: Configuración → Buscar actualización → Descargar actualización → Aplicar y reiniciar. Desde ModsEx 1.4.2 las actualizaciones se aplican en modo silencioso; la descarga diferencial depende de los paquetes disponibles y puede recurrir al paquete completo.
- Inicio muestra solo seis destacados. Mi colección contiene la lista completa debajo del panel de Mods locales.

## Borrar un mod del PC

Cierra Minecraft. Mi colección → Mods locales → Actualizar lista → selecciona el archivo → Borrar seleccionados del PC. Confirma los nombres y la carpeta. Los archivos van a la Papelera. Esto no cambia Aternos ni el catálogo; si siguen publicados, volverán a figurar como pendientes.

## Controles útiles

- Player Emotes: B por defecto. Si JourneyMap también usa B, cambia una de las asignaciones en Opciones → Controles.
- Inventory HUD+: O por defecto. Si no aparece en la lista Mods de Minecraft, revisa que descargaste el JAR en la carpeta del perfil que estás ejecutando y reinicia el juego.
- FPS Reducer: ahorra recursos cuando el juego está inactivo o minimizado; no aumenta FPS durante juego activo.

Los mods exclusivos de servidor se documentan en `server-mods.json`; no uses ese archivo como catálogo de descargas para los PCs. La compatibilidad declarada y los archivos se han verificado, pero no se ha realizado una prueba de juego completa de esta combinación en todos los equipos.
