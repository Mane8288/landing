# Soporte de controles

<Alert variant="warning">

Debes desactivar el soporte de controles de Steam (o salir completamente de Steam) antes de probar controles en Plutonium.  
Simplemente ve a Configuración de Steam -> Controles -> Configuración general del control y **desmarca** las casillas como se muestra a continuación:

![disablesteamcontroller](/images/docs/controllers/U1bs5Z9.png)

</Alert>

## Controles de Xbox

Los controles de Xbox deberían funcionar sin problemas con todos nuestros juegos.  
Simplemente conecta tu control a tu computadora y abre Plutonium.

## Controles de PS4 y PS5

Los controles de PS4 y PS5 requieren un software adicional para funcionar fuera de Steam en Windows.

1\. Descarga [DS4Windows](https://github.com/Ryochan7/DS4Windows/releases/latest). Recomendamos descargar `DS4Windows_VERSION_x64.zip`.

2\. Abre el archivo zip descargado y copia la carpeta `DS4Windows` a un lugar seguro, como tu carpeta de Documentos.

3\. Abre la carpeta extraída y luego abre `DS4Windows`

![img](/images/docs/controllers/sxik1Bs.png)

4\. Si aparece un mensaje como este, haz clic en `Sí`.

![error](/images/docs/controllers/BEqRTW4.png)

4a\. Debería abrirse tu navegador y debes descargar la versión de Windows x64.

![img](/images/docs/controllers/s2FRt73.png)

4b\. Abre e instala .NET.

4c\. Si aún obtienes un error similar al paso 4, simplemente descarga y ejecuta el .NET redist que se muestra en la página de lanzamiento (la página que se abrió en el paso 1).

5\. Después de la instalación, vuelve a intentar con DS4Windows.

6\. Selecciona `Appdata` como ruta de guardado.

![img](/images/docs/controllers/3EJ1wzA.png)

7\. Instala el controlador ViGEmBus.

![img](/images/docs/controllers/RHrY0Wu.png)

8\. Conecta tu control de PS4 a tu PC.
Si estás utilizando Bluetooth, sigue las indicaciones dentro de DS4Windows.

9\. Una vez conectado, haz clic en "Finalizar" en la pantalla de Bienvenido a DS4Windows.

10\. Configura tu control y ejecuta DS4Windows en la ventana principal.

11\. ¡Entra al juego y verifica si tu control funciona!

Ten en cuenta que DS4Windows debe estar en ejecución para detectar tu control, así que asegúrate de habilitarlo al iniciar en la configuración.

![img](/images/docs/controllers/ps4-final.png)

## Controles de PS3

Al igual que con otros controles de PlayStation, los controles de PS3 requieren un software adicional para funcionar fuera de Steam en Windows.
Existen varias herramientas que puedes utilizar para hacer funcionar tu control de PS3, pero en esta guía utilizaremos ScpToolkit.

1\. Descarga [ScpToolkit](https://github.com/nefarius/ScpToolkit/releases/download/v1.7.277.16103-BETA/ScpToolkit_Setup.exe).

2\. Abre el archivo de instalación descargado y haz clic en "Siguiente" sin cambiar ninguna configuración. Al final, haz clic en "Run Driver Installer" (Ejecutar instalador de controles).

3\. Sigue todas las instrucciones en pantalla y asegúrate de leer todo (inicializa el control Dualshock e instala los controles requeridos). Hacer clic en "Siguiente" no instalará nada, debes hacer clic en los botones de instalación que se muestran en pantalla, como se muestra en la captura de pantalla a continuación. Puedes omitir las instalaciones que no necesites, como Bluetooth.

![img](/images/docs/controllers/ps3-1.png)

Si tu control aún no funciona, puedes abrir la aplicación "ScpServer" (que se encuentra en la carpeta ScpToolkit) y ejecutarla manualmente si aún no se ha iniciado.
La aplicación "ScpSettings" te permitirá cambiar configuraciones, como habilitar/deshabilitar la vibración, cambiar la zona muerta de los joysticks y otras opciones.

## Mi control aún no funciona

### Cualquier control

Primero, asegúrate de que el control esté habilitado en la configuración del juego. Esto generalmente se encuentra en Configuración > Controles > Gamepad.

También recomendamos probar tu control en un juego en lugar de en los menús, ya que no todos los juegos admiten/soportan completamente los controles en los menús.

Por último, asegúrate de que has desactivado las configuraciones correctas en Steam, como se menciona al principio de esta página, o que has salido completamente de Steam haciendo clic derecho en el icono de Steam en el menú de la bandeja del sistema de Windows y seleccionando "Salir".

### DS4Windows

Si estás utilizando DS4Windows, asegúrate de seleccionar el perfil predeterminado.  
![img](/images/docs/controllers/ds4windows-main.png)

Luego haz clic en el botón "Editar", ve a la pestaña llamada "Other" (en la parte derecha) y asegúrate de que "Emulated Controller" esté configurado como Xbox 360.  
![img](/images/docs/controllers/ds4windows-profile.png)

### World at War

Si crees que has hecho todo correctamente y tu controlador aún no funciona en World at War, puedes intentar [aplicar la configuración del controlador del juego](/docs/client/t4/rebinding-controller/).

## Cambiar la acción de recarga

Los usuarios de controladores están acostumbrados a utilizar el botón X / Cuadrado para recargar, pero también lo mantienen presionado para realizar la acción de "uso".
En el teclado, estos se intercambian por teclas separadas, por defecto R para recargar y F para usar.

Para intercambiarlos, sigue estos pasos:

1. [Abre la consola](/docs/opening-console)
2. Ingresa lo siguiente:
```cs
bind r +usereload
```
Ahora, R debería haber sido intercambiado por +usereload en lugar de +reload. Asegúrate de que tu controlador esté asignado al botón R y deberías estar bien.

## Cambiar los gatillos/botones superiores

Puedes intercambiar los gatillos y los botones superiores [abriendo la consola](/docs/opening-console) y pegando esto:

```cs
bind BUTTON_LSHLDR "+speed_throw"; bind BUTTON_RSHLDR "+attack"; bind BUTTON_LTRIG "+smoke"; bind BUTTON_RTRIG "+frag"
```