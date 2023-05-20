# Cómo evitar que tu juego se vea ampliado

Si tu juego se ve ampliado como se muestra en la captura de pantalla de abajo, incluso cuando la resolución del juego no es mayor que la resolución de tu monitor, es posible que esto solucione tu problema.

![img](/images/docs/fix-game-zoomed-in/example.png)

## ¿Por qué ocurre esto?

Esto sucede porque tu configuración de escala en Windows está establecida en un valor superior al 100% y algunos juegos utilizarán esa configuración de escala, pero puedes evitar que eso suceda.
![img](/images/docs/fix-game-zoomed-in/windows-setting.png)

## Cómo solucionarlo

En primer lugar, intenta presionar ALT+Enter para ver si el juego se fuerza a pantalla completa. Si no, continúa leyendo.

La solución que se presenta a continuación solo cambiará la configuración para los juegos de Plutonium, manteniendo intacta la configuración de escala de Windows para todas las demás aplicaciones.

1. Asegúrate de que el iniciador de Plutonium y cualquier juego de Plutonium estén cerrados.

2. Presiona Win + R, pega `%localappdata%\Plutonium\bin` y presiona Enter.

3. Haz clic derecho en `plutonium-bootstrapper-win32` y selecciona `Propiedades`.

4. Ve a la pestaña `Compatibilidad` y haz clic en `Cambiar configuración elevada de PPP`.

5. Marca la casilla `Invalidar el comportamiento de ajuste con valores altos de PPP`.

6. En `Ajuste realizado por`, selecciona `Aplicación`. Si ya estaba configurado en `Aplicación`, prueba con la(s) otra(s) opción(es).

![img](/images/docs/fix-game-zoomed-in/app-setting.png)

7. Abre el iniciador nuevamente y ejecuta tu juego para ver si se ha solucionado el problema.
