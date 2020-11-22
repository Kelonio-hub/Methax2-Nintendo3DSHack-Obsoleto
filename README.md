# Methax
Método de modificación de consola 3Ds

Methax es un proceso de modificación de la consola 3Ds que mezcla parte del proceso Pichaxx [https://gist.github.com/zoogie/931c87ca8cae98c28e931182af26f89b] 
y parte del proceso USM [https://github.com/zoogie/unSAFE_MODE]. Ambos procesos son del dev Zoogie y todos los agradecimientos son para él y su gran trabajo. 
Este repositorio sólo es un conjunto de pasos creados por Zoogie que nacen de la necesidad de hackear la consola 3Ds en la nueva versión 11.14. 

En primer lugar, necesitaremos: 
- 3ds/2ds de modelo Old o New y en región U/E/J.
- Descargar el juego Pokemon Picross desde la eshop (para consolas de residencia en LATAM deberán cambiar su residencia a EEUU).
- Apuntar nuestro código de amigo. 

En segundo lugar, acudiremos a: 
- https://bruteforcemovable.com/ para sacar el archivo .sed (se obtiene añadiendo el código de amigo y los dígitos de la primera carpeta que está en el interior de Nintendo 3ds)
- https://3ds.hobbyist.dev/3dstools/pichaxx.php para sacar el archivo .sav (se obtiene añadiendo el .sed anterior). Este .sav debemos meter en la siguiente ruta: 
sdmc:/Nintendo 3DS/long hex number/another long hex number/title/00040000/0017c100/data/ y remplazar el ya existente. 
- https://deadphoenix8091.github.io/3ds/#otherapp para sacar el .bin que deberemos renombrar por otherapp u otherapp.bin. Dicho archivo irá a la raíz de la Sd. 

En tercer lugar, introduciremos los archivos hack (se encuentra luma 10.2.1 y godmode9 1.9.2) en la raíz de la sd: https://mega.nz/file/6l821ZzK#83ybuL7ZBbbGEGmRtFXkI6E_Zt8rI7JbwwXlAaiYBQs

En cuarto lugar, acudiremos a la consola y abriremos el juego de Pokemon Picross. En esta ocasión se flasheará y saldrá el Homebrew Launcher. 
A continuación, ejecutaremos el programa TWLfix.3dsx para verificar tener activas las conexiones.
Posteriormente, ejecutaremos el programa SlotTool para modificar las conexiones. Éstas serán renombradas por HAXXXXXXXX.
Apagaremos la consola y acudiremos al modeo recóvery (L+R+A+Up+Power). 

1. ¿Quieres conectarte a internet para actualizar la consola? Aceptar. Lanzará un error 003-1099, es algo común. 

2- ¿Quieres configurar tu conexión a internet? Aceptar. 

3- seleccionar Conexión 1. Modificar ajustes. Segunda página. Servidor Proxy. Ajustes avanzados. La consola se flasheará de nuevo y se acabá de instalar el Boot9

En quinto Lugar, saldrá el menú de Luma (de no ser así lo abriremos con select+power) y marcaremos la opción: Show current NAND in System Settings

Por último, quedará: 
1. Instalar el FBI desde el godmode9 o mediante Rosalina. 
2. Restablecer las conexiones: abriremos el homebrew launcher (mediante rosalina o mediante .cia), ejecutamos SlootTool y elegimos la opción Restore Wifi. 
3. Crear respaldo NAND. 
