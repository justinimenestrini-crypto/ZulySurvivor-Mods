# ZulySurvivor: Fabric 1.21.11

## Estado

El catálogo del PC está preparado para Fabric. El servidor de Aternos seguía en Forge 61.2.0 y en línea al revisar la migración. `server-mods.json` describe el destino previsto y no acredita una instalación realizada.

Usar Java 21 y Fabric Loader 0.18.4 o superior; Aternos ofrece 0.19.5 como recomendada para Minecraft 1.21.11.

## En cada PC

1. Cerrar Minecraft. Crear un perfil independiente de Minecraft 1.21.11 con Fabric. Elegir su carpeta real de juego; no reutilizar una carpeta con archivos Forge.
2. En ModsEx, Configuración: elegir Fabric, Minecraft 1.21.11 y la carpeta `mods` del perfil Fabric; guardar.
3. Mi colección → Comprobar → Instalar faltantes. La colección toma el cargador de `mods.json`.
4. Los JAR Forge que ya estaban descargados NO se borran al cambiar el catálogo. Si se reutiliza una carpeta, seleccionar únicamente esos JAR en Mods locales y moverlos a la Papelera después de guardar copia. No borrar mundos, capturas ni configuraciones.
5. Iniciar con el perfil Fabric. Un cliente Fabric con mods obligatorios no debe intentar conectarse al antiguo servidor Forge.

## Rendimiento incluido

| Mod | Versión | Destino | Función |
|---|---|---|---|
| Sodium | 0.8.14 | PC | Renderizado y FPS |
| ImmediatelyFast | 1.14.3 | PC | Renderizado inmediato |
| More Culling | 1.6.2 | PC | Reduce caras ocultas; necesita Cloth Config |
| BadOptimizations | 2.4.1 | PC | Evita trabajo innecesario |
| Lithium | 0.21.4 | PC y servidor, independientes | Lógica del juego |
| FerriteCore | 8.2.0 | PC y servidor, independientes | Uso de memoria |
| Krypton | 0.2.10 | PC y servidor, independientes | Red, no aumento de FPS garantizado |
| Adaptive Performance Tweaks | 12.10.0 | Servidor | Gestión de carga; se conserva la selección anterior |
| Clumps | 29.0.0.1 | Utilidad principalmente en servidor | Orbes de experiencia |
| FPS Reducer | 2.15 | PC | Ahorra recursos en pausas; no aumenta FPS al jugar |

Se conservan JourneyMap, Extended ItemView, Balm, Waystones, Player Emotes e Inventory HUD+ con archivos Fabric, además de Fabric API y Cloth Config como bibliotecas. Skin Restorer se incluye solo en la lista prevista del servidor.

## Exclusiones

- Punchy continúa excluido por la petición anterior del administrador.
- Entity Culling 1.11.3 declara `breaks: {tlskincape: "*"}` en su `fabric.mod.json`. No se incluye por el uso de TLauncher.
- No se combinan Sodium y OptiFine/OptiFabric, Embeddium o VulkanMod.
- No se añaden a la vez varios controladores adaptativos del servidor. ServerCore no se añade encima de Adaptive Performance Tweaks.
- Ksyxis apareció en el servidor Forge, pero no se arrastra sin una revisión específica de Fabric y de sus efectos sobre la carga de chunks.

## En Aternos

Guardar un respaldo antes de cambiar el cargador. Revisar cualquier aviso de Aternos antes de aplicar una reinstalación. Instalar únicamente desde su catálogo, sin subir JAR ni eludir restricciones. Los mods de PC como Sodium e ImmediatelyFast no se instalan en Aternos.

La lista `server-mods.json` contiene los archivos Fabric previstos. Hay que comprobar disponibilidad de cada versión en Aternos y verificar los JAR reales tras instalar. Mantener el servidor detenido durante la sustitución de archivos Forge por Fabric. Revisar el registro de inicio antes de invitar a los jugadores.

## Validación realizada

Se consultaron versiones estables de Modrinth para Fabric 1.21.11; se descargaron sin ejecutarlos los JAR seleccionados para comprobar SHA-512, `fabric.mod.json`, Java, Loader, dependencias y conflictos declarados. Se comprobó que el planificador de ModsEx resuelve 17 archivos únicos del catálogo y excluye la lista del servidor de las descargas del PC.

Esto es validación estática; no equivale a una prueba de arranque de Minecraft ni a una medición de FPS en los equipos de los jugadores.
