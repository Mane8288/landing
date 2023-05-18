# ¿Cómo instalar Plutonium?

## Iniciador de Plutonium

1. Descarga [plutonium.exe](https://cdn.plutonium.pw/updater/plutonium.exe)

Puedes guardar el iniciador donde quieras, como tu escritorio o la carpeta del juego.

2. Ahora, abre el iniciador. Si aparece el Smart Screen de Windows, da click en **Más información**, luego en **Ejecutar de todas formas**.

![smartscreen 1](/images/docs/install/QVb7Cv4.png)
![smartscreen 2](/images/docs/install/E4lDWsb.png)

El iniciador ahora empezará a instalar los archivos del cliente.

![launcher self update / installation](/images/docs/install/9aHmzEk.png)

3. Ingresa tus credenciales del foro para iniciar sesión. Si todavía no tienes una cuenta en el foro, puedes crear una [aquí](https://forum.plutonium.pw/register).

![launcher login page](/images/docs/install/sA951Dt.png)

4. Configura el juego que desees jugar.

## T6 (Black Ops 2)

### Solo quiero actualizar / ya tengo Black Ops 2 instalado

Si ya tienes el juego instalado en Steam o una actualización anterior de Plutonium, entonces puedes saltarte la sección de abajo e ir directo a la **[Instalación de DLCs](#installing-t6-dlc)**.

### Para instalar el juego base (BO2)

Esta sección crubrirá la descarga de una copia de BO2. Por favor, salta esta parte si ya tienes una copia de BO2.

**Nótese que recomendamos que compres el juego si no lo tienes. Esta es la mejor manera de conseguir una copia del juego que no esté corrupta o alterada de alguna forma. Algunos sitios ofrecen descuentos decentes.**

1. Desde el explorador de Windows ve a Mi Equipo, despues a **Windows (C:)** y crea una carpeta llamada `Games`

![Explorer steps 1-2](/images/docs/install/bmMI4UH.png)

![Explorer step 3](/images/docs/install/1MphGAa.png)

![Explorer step 4](/images/docs/install/cRa2jC2.png)

<Alert variant="warning">

¡El torrenting de archivos protegidos con Copyright puede ser ilegal en tu país, incluso si tienes una licencia válida!
No nos hacemos responsables por cualquier problema legal y recomendamos una <a href="steam://install/202990">descarga nueva desde Steam</a> o un VPN.

</Alert>

2. Descarga/abre tu programa de torrent preferido.
Recomendamos qBittorent Windows x64: [https://www.fosshub.com/qBittorrent.html](https://www.fosshub.com/qBittorrent.html)

3. Descarga el [archivo torrent](/pluto_t6_full_game.torrent).

4. Abre el archivo `pluto_t6_full_game.torrent` (del paso anterior). Abrirá tu cliente torrent preferido y te preguntará dónde quieres guardar el juego.
**SELECCIONA LA CARPETA 'Games' QUE CREASTE EN EL PASO 1**

5. Inicia la descarga y espera a que termine. Sabrás que terminó cuando el progreso marque `100%` y el estado cambie a `Seeding` o `Sembrando`.

Cuando termine, tendrás tu copia del juego descargada. Aquí hay un ejemplo de una carpeta de juego completa:

![Completed Game Folder](/images/docs/install/B8g1bXI.png)

### Instalación de los DLCs (BO2)

<Alert variant="warning">

Si instalaste el juego utilizando el torrent de las instrucciones de arriba, entonces [pasa a configurar el iniciador](#setting-up-t6-with-the-plutonium-launcher).  
**Esto es solo para aquellos que usaron los archivos de Steam, pero no tienen ningún DLC**.  
Esto solo descarga los mapas de DLC. No puedes jugar el juego solo con estos archivos. Si quieres descargar el juego, entonces [lee arriba](#installing-the-base-game-bo2)!  
Ten en cuenta que si un servidor rota sus mapas a uno de DLC y no los tienes instalados, el juego te expulsará, así que si puedes instalarlos, hazlo.  

</Alert>

1. Descarga/abre tu programa de torrent preferido.
Recomendamos qBittorent Windows x64: [https://www.fosshub.com/qBittorrent.html](https://www.fosshub.com/qBittorrent.html)

2. Descarga el [archivo torrent](/t6_dlcs.torrent).

3. Abre el archivo `t6_dlcs.torrent` (del paso anterior). Abrirá tu cliente torrent preferido y te preguntará dónde quieres guardar los DLC.
**SELECCIONA TU CARPETA DE BO2 DE STEAM**

![img](/images/docs/install/9ff55628c526220795c0f23f3a6aa719.png)

4. Selecciona `"no crear subcarpeta"` del menú desplegable en `"Diseño de contenido"` (en versiones más antiguas de qBittorent estará la opción `"crear subcarpeta"` o `"mantener carpeta de nivel superior"`, la cual debes desmarcar)

![img](/images/docs/install/f32c04d072946509231016a435e9c521.png)

5. Inicia la descarga y espera a que termine. 
Sabrás que terminó cuando el progreso marque `100%` y el estado cambie a `Seeding` o `Sembrando`.

### Configuración de T6 con el iniciador de Plutonium

Navega a Black Ops 2 y presiona **SETUP**. Luego selecciona tu carpeta de Black Ops 2. 
La carpeta que necesitas seleccionar muy probablemente se llama `pluto_t6_full_game` o `Call of Duty Black Ops II`.
No selecciones la carpeta Games o tu carpeta Documentos. **Selecciona la carpeta que contiene los archivos de Black Ops II!**

![Launcher set-up 1](/images/docs/install/5FOePMY.png)

* **Si estás usando una copia de Steam, el juego estará en la siguiente ruta:** `{Letra del disco}\Program Files (x86)\Steam\steamapps\common\Call of Duty Black Ops 2`

* **Si usaste el torrent, el juego estará en una carpeta llamada** `pluto_t6_full_game`
![Launcher set-up 2](/images/docs/install/hdjiIhN.png)

**Si alguna vez necesitas reseleccionar la carpeta del juego, simplemente dale click al ícono de la tuerca al lado del botón que dice PLAY**
![Launcher reselect hint](/images/docs/install/MnkAcr8.png)

Para aquellos que tienen problemas en localizar sus archivos del juego, así es como se ve el contenido de su carpeta:

![Completed Game Folder](/images/docs/install/B8g1bXI.png)

### Error de T6: Invalid Game Path (Ruta de juego inválida)

Como dice el error, seleccionaste una ruta inválida para tu juego.

![img](/images/docs/install/46KPMDc.png)

Si salta este error, significa que seleccionaste tu disco en vez de la carpeta del juego. 
`C:\` no es la carpeta de Black Ops II. 

![img](/images/docs/install/error-401.png)

En ambos casos, la manera de arreglar este error es darle clic en Game settings (Configuración de juego) en el iniciador y seleccionar la carpeta que contiene los archivos de Black Ops II.
Si no puedes encontrar la carpeta, entonces lee la [guía desde el comienzo](#t6-black-ops-2) de nuevo.

![img](/images/docs/install/MnkAcr8.png)

¡Felicitaciones! Completaste la guía de instalación.

Para ejecutar Black Ops II, simplemente abre el iniciador de Plutonium y dale clic en PLAY.

---

## IW5 (Modern Warfare 3)

### Solo quiero actualizar / ya tengo MW3 instalado

Si ya tienes el juego instalado en Steam o una actualización anterior de Plutonium, entonces puedes saltarte la sección de abajo e ir directo a la [Instalación de DLCs](#installing-the-dlc).

### Installing the base game (MW3)

Nota: Esta sección crubrirá la descarga de una copia GRATIS de MW3. Por favor, salta esta parte si ya tienes una copia de MW3.

Por favor ten en cuenta que recomandamos comprar el juego si no lo tienes. Si disfrutas de un juego, apoya a sus desarrolladores.

Abre Steam. Si no lo tienes instalado, puedes hacerlo [aquí](https://store.steampowered.com/about/).

#### Método 1

Dale clic a este link para comenzar la instalación de Call of Duty: Modern Warfare 3 - Dedicated Server en Steam: [steam://install/42750](steam://install/42750).

#### Método 2 (Si el Método 1 no funciona)

1. Ves a `BIBLIOTECA` y desde el menú desplegable selecciona `HERRAMIENTAS`.

![img](/images/docs/install/fzKXqGs.png)

2. Localiza `Call of Duty: Modern Warfare 3 - Dedicated Server`, selecciónalo y dale clic al ícono de la tuerca. Luego ve a `Propiedades`.

![img](/images/docs/install/ln7ml3F.png)

3. Navega a la ventana de `IDIOMA` y asegúrate de que el lenguaje sea `INGLÉS`. Esto es muy importante debido a que desafortunadamente el MW3 Dedicated Server de Steam no puede instalar todos los lenguajes, lo que resultaría en archivos faltantes / errores.

![img](/images/docs/install/NXLe3YD.png)

<Alert variant="tip">

Si quieres el juego en tu lenguaje nativo, sugerimos comprar el juego y sus DLCs en un sitio clave o durante una oferta de Steam.

</Alert>

4. Selecciona `INSTALAR`, luego `Siguiente`, después `Finalizar`.

![img](/images/docs/install/LVhQAtW.png)

![img](/images/docs/install/pQB76hJ.png)

Ahora solo espera a que se complete la descarga, la cual puedes monitorear dándole clic al texto `DESCARGAS` en la zona inferior de la interfaz de Steam. Una vez se complete la descarga, tendrás una copia de MW3

### Instalación de los DLC (MW3)

Esta sección cubrirá cómo descargar e instalar los DLC en Inglés para obtener la experiencia completa de MW3.  
Si no quieres instalarlos, entonces puedes [saltar a la configuración en el iniciador](#setting-up-iw5-with-the-plutonium-launcher).  
Puedes descargarlos usando el lunk de MEGA o el torrent. **No tienes que descargar los dos, solo escoge el que funcione mejor para ti.**  
Nótese que estos archivos solo funcionarán en una copia en Inglés del juego y son opcionales. Descárgalos únicamente si deseas jugar los mapas de DLC.  
Ten en cuenta que si un servidor rota sus mapas a uno de DLC y no los tienes instalados, el juego te expulsará, así que si puedes instalarlos, hazlo.   
Esto solo descarga los mapas de DLC. No puedes jugar el juego solo con estos archivos. Si quieres descargar el juego, entonces [lee arriba](#installing-the-base-game-mw3)!

#### MEGA

1. Descarga el archivo zip de los DLC usando el siguiente [link](https://mega.nz/folder/CYUkGSrJ#HVa6Cik59Bgi9pp5NBW4fg).

![img](/images/docs/install/Zqx80uj.png)

2. Una vez completada la descarga, abre el zip `MW3 DLC [EN].zip`

![img](/images/docs/install/4ty889E.png)

![img](/images/docs/install/9wYQgJ3.png)

3. Localiza tu carpeta de MW3 en el explorador de archivos.
Steam la tendrá instalada en la siguiente ruta por defecto: `C:\Program Files (x86)\Steam\steamapps\common\Call of Duty Modern Warfare 3`
También puedes encontrar tu carpeta desde Steam si es necesario

![img](/images/docs/install/K7dj3mP.png)


4. Ahora regresa al archivo `MW3 DLC [EN].zip` y arrastra y suelta las carpetas `main` y `zone` dentro de tu carpeta de MW3.
En caso de que se te pregunte, `reemplaza todos los archivos en el destino`.

![img](/images/docs/install/3m5tWAj.png)

![img](/images/docs/install/yKw8Rl2.png)

#### Torrent

1. Descarga/abre tu programa de torrent preferido.
Recomendamos qBittorent Windows x64: [https://www.fosshub.com/qBittorrent.html](https://www.fosshub.com/qBittorrent.html)

2. Descarga el [archivo torrent](/iw5m_dlcs.torrent).

3. Abre el archivo `iw5m_dlcs.torrent` (del paso anterior). 
Abrirá tu cliente torrent preferido y te preguntará dónde quieres guardar los DLC.
**SELECCIONA TU CARPETA DE MW3**

Steam la tendrá instalada en la siguiente ruta por defecto: `C:\Program Files (x86)\Steam\steamapps\common\Call of Duty Modern Warfare 3`
También puedes encontrar tu carpeta desde Steam si es necesario

![img](/images/docs/install/K7dj3mP.png)

![img](/images/docs/install/mw3_torrent_folder.png)

4. Selecciona `"no crear subcarpeta"` del menú desplegable en `"Diseño de contenido"` (en versiones más antiguas de qBittorent estará la opción `"crear subcarpeta"` o `"mantener carpeta de nivel superior"`, la cual debes desmarcar)

![img](/images/docs/install/f32c04d072946509231016a435e9c521.png)

5. Desmarca `iw5m_dlcs`. Marca `main` y `zone`.

![img](/images/docs/install/mw3_torrent_settings.png)

6. Inicia la descarga y espera a que termine. 
Sabrás que terminó cuando el progreso marque `100%` y el estado cambie a `Seeding` o `Sembrando`.

¡Felicidades! Ahora los DLC están instalados.

### Configuración de IW5 con el iniciador de Plutonium

Navega a Modern Warfare 3 y presiona **SETUP**. Luego, selecciona tu carpeta de Modern Warfare 3. 
La carpeta que necesitas seleccionar se llama `Call of Duty Modern Warfare 3`.
No selecciones la carpeta Games o tu carpeta Documentos. **Selecciona la carpeta que contiene los archivos de Modern Warfare 3!**
![img](/images/docs/install/qDJ7OeD.png)

* **Si seguiste la guía al pie de la letra, estará en esta ruta:** `C:\Program Files (x86)\Steam\steamapps\common\Call of Duty Modern Warfare 3`.

![img](/images/docs/install/qtgfVmJ.png)

**Si alguna vez necesitas reseleccionar la carpeta del juego, simplemente dale click al ícono de la tuerca al lado del botón que dice PLAY**
![img](/images/docs/install/MnkAcr8.png)

Para aquellos que tienen problemas en localizar sus archivos del juego, así es como se ve el contenido de su carpeta:

![img](/images/docs/install/7FOyDlg.png)

### Error de IW5: Invalid Game Path (Ruta de juego inválida)

Como dice el error, seleccionaste una ruta inválida para tu juego, por lo que esta no contiene los archivos del juego.

![img](/images/docs/install/mw3-wrong-folder.png)

Si salta este error, significa que seleccionaste tu disco en vez de la carpeta del juego. 
`C:\` no es la carpeta de Modern Warfare 3. 

![img](/images/docs/install/error-401.png)

En ambos casos, la manera de arreglar este error es darle clic en Game settings (Configuración de juego) en el iniciador y seleccionar la carpeta que contiene los archivos de Modern Warfare 3.
Si no puedes encontrar la carpeta, entonces lee la [guía desde el comienzo](#iw5-modern-warfare-3) de nuevo.

![img](/images/docs/install/MnkAcr8.png)

¡Felicitaciones! Completaste la guía de instalación.

Para ejecutar Modern Warfare 3, simplemente abre el iniciador de Plutonium y dale clic en PLAY.

<Alert variant="warning">
El juego va a crashear la primera vez que lo ejecutes debido a que necesita borrar un archivo, así que solo ejecútalo de nuevo y no volverás a ver este error.
</Alert>

---

## T4 (World at War)

### Solo quiero actualizar / ya tengo WaW instalado

Si ya tienes el juego instalado en Steam, entonces puedes saltarte la sección de abajo e ir al sección del [Iniciador de Plutonium](#setting-up-t4-with-the-plutonium-launcher).

### ***Instalación del juego base (WaW)***

Esta sección crubrirá la descarga de una copia de WaW. Por favor, salta esta parte si ya tienes una copia de WaW.

Nótese que recomendamos que compres el juego si no lo tienes. Esta es la mejor manera de conseguir una copia del juego que no esté corrupta o alterada de alguna forma. Algunos sitios ofrecen descuentos decentes.

1. Crea una carpeta llamada `Games`en cualquier disco.

2. Desde el explorador de Windows ve a Mi Equipo, despues a Windows (C:) y crea una carpeta llamada `Games`.
![PC Explorer](/images/docs/install/bmMI4UH.png)
![Games Folder](/images/docs/install/1MphGAa.png)
![Games Folder Completed](/images/docs/install/cRa2jC2.png)

<Alert variant="warning">

¡El torrenting de archivos protegidos con Copyright puede ser ilegal en tu país, incluso si tienes una licencia válida!
No nos hacemos responsables por cualquier problema legal y recomendamos una <a href="steam://install/10090">descarga nueva desde Steam</a> o un VPN.

</Alert>

3.  Descarga/abre tu programa de torrent preferido.
Recomendamos [qBittorent Windows x64](https://www.fosshub.com/qBittorrent.html).

4. Descarga el [archivo Torrent](/pluto_t4_full_game.torrent).

5. Abre el archivo torrent (del paso anterior). Abrirá tu cliente torrent preferido y te preguntará dónde quieres guardar el juego.

**SELECCIONA LA CARPETA 'Games' QUE CREASTE EN EL PASO 1**

6. Inicia la descarga y espera a que termine. Sabrás que terminó cuando el progreso marque `100%` y el estado cambie a `Seeding` o `Sembrando`.

**Cuando diga "Sembrando", podrás borrarlo de qBittorrent.**

Cuando termine, tendrás tu copia del juego descargada. Aquí hay un ejemplo de una carpeta de juego completa:

![Completed T4 Folder](/images/docs/install/NoAuNW8.png)

---

### Configuración de T4 con el iniciador de Plutonium

Navega a World at War y presiona **SETUP**. Luego selecciona tu carpeta de World at War. 
La carpeta que necesitas seleccionar muy probablemente se llama `pluto_t4_full_game` o `Call of Duty World At War`. 
No selecciones la carpeta Games o tu carpeta Documentos. **Selecciona la carpeta que contiene los archivos de World at War!**
![WAW in launcher](/images/docs/install/4xzmAUX.png)

Si estás usando una copia de Steam, el juego estará en la siguiente ruta: `C:\Program Files (x86)\Steam\steamapps\common\Call of Duty World At War`

Si usaste el torrent, el juego estará en una carpeta llamada `pluto_t4_full_game`

(Si alguna vez necesitas reseleccionar la carpeta del juego, simplemente dale click al ícono de la tuerca al lado del botón que dice PLAY)

---

### Error de T4: Invalid Game Path (Ruta de juego inválida)

Como dice el error, seleccionaste una ruta inválida para tu juego, por lo que esta no contiene los archivos del juego.

![Invalid Game Directory](/images/docs/install/vlwamKe.png)

Si salta este error, significa que seleccionaste tu disco en vez de la carpeta del juego. 
`C:\` no es la carpeta de World at War.

![img](/images/docs/install/error-401.png)

En ambos casos, la manera de arreglar este error es darle clic en Game settings (Configuración de juego) en el iniciador y seleccionar la carpeta que contiene los archivos de World at War.
Si no puedes encontrarla, entonces lee la [guía desde el comienzo](#t4-world-at-war) de nuevo.

![img](/images/docs/install/MnkAcr8.png)

---

**¡Felicitaciones! Completaste la guía de instalación.**

Para ejecutar World at War, simplemente abre el iniciador de Plutonium y dale clic en PLAY.

## T5 (Black Ops 1)

### ***Solo quiero actualizar / ya tengo WaW instalado***

Si ya tienes el juego instalado en Steam o una actualización anterior de Plutonium, entonces puedes saltarte la sección de abajo e ir directo a la **[Instalación de DLCs](#installing-the-dlcs-bo1)**.

### ***Instalación del juego base (BO1)***

Esta sección crubrirá la descarga de una copia de BO1. Por favor, salta esta parte si ya tienes una copia de BO1.

Nótese que recomendamos que compres el juego si no lo tienes. Esta es la mejor manera de conseguir una copia del juego que no esté corrupta o alterada de alguna forma. Algunos sitios ofrecen descuentos decentes.

1. Crea una carpeta llamada `Games`en cualquier disco.

2. Desde el explorador de Windows ve a Mi Equipo, despues a Windows (C:) y crea una carpeta llamada `Games`.
![PC Explorer](/images/docs/install/bmMI4UH.png)
![Games Folder](/images/docs/install/1MphGAa.png)
![Games Folder Completed](/images/docs/install/cRa2jC2.png)

<Alert variant="warning">

¡El torrenting de archivos protegidos con Copyright puede ser ilegal en tu país, incluso si tienes una licencia válida!
No nos hacemos responsables por cualquier problema legal y recomendamos una <a href="steam://install/10090">descarga nueva desde Steam</a> o un VPN.

</Alert>

3. Descarga/abre tu programa de torrent preferido.
Recomendamos [qBittorent Windows x64](https://www.fosshub.com/qBittorrent.html).

4. Descarga el [archivo Torrent](/pluto_t5_full_game.torrent).

5. Abre el archivo torrent (del paso anterior). Abrirá tu cliente torrent preferido y te preguntará dónde quieres guardar el juego.

**SELECCIONA LA CARPETA 'Games' QUE CREASTE EN EL PASO 1**

6. Inicia la descarga y espera a que termine. Sabrás que terminó cuando el progreso marque `100%` y el estado cambie a `Seeding` o `Sembrando`.

**Cuando diga "Sembrando", podrás borrarlo de qBittorrent.**

Cuando termine, tendrás tu copia del juego descargada. Aquí hay un ejemplo de una carpeta de juego completa:

![Completed T5 Folder](/images/docs/install/NoAuNW9.png)

---

### Instalación de los DLC (BO1)

<Alert variant="warning">

Si instalaste el juego utilizando el torrent de las instrucciones de arriba, entonces [pasa a configurar el iniciador](#setting-up-t5-with-the-plutonium-launcher).  
**Esto es solo para aquellos que usaron los archivos de Steam, pero no tienen ningún DLC**.  
Esto solo descarga los mapas de DLC. No puedes jugar el juego solo con estos archivos. Si quieres descargar el juego, entonces [lee arriba](#installing-the-base-game-bo1)!  
Ten en cuenta que si un servidor rota sus mapas a uno de DLC y no los tienes instalados, el juego te expulsará, así que si puedes instalarlos, hazlo.  

</Alert>

1. Descarga/abre tu programa de torrent preferido.
Recomendamos qBittorent Windows x64: [https://www.fosshub.com/qBittorrent.html](https://www.fosshub.com/qBittorrent.html)

2. Descarga el [archivo torrent](/t5_dlcs.torrent).

3. Abre el archivo `t5_dlcs.torrent` (del paso anterior). Abrirá tu cliente torrent preferido y te preguntará dónde quieres guardar los DLC.
**SELECCIONA TU CARPETA DE BO1**

![img](/images/docs/install/bo1-qb.png)

4. Selecciona `"no crear subcarpeta"` del menú desplegable en `"Diseño de contenido"` (en versiones más antiguas de qBittorent estará la opción `"crear subcarpeta"` o `"mantener carpeta de nivel superior"`, la cual debes desmarcar)

![img](/images/docs/install/f32c04d072946509231016a435e9c521.png)

5. Inicia la descarga y espera a que termine. 
Sabrás que terminó cuando el progreso marque `100%` y el estado cambie a `Seeding` o `Sembrando`.

---

### Configuración de T5 con el iniciador de Plutonium

Navega a Black Ops y presiona **SETUP**. Luego selecciona tu carpeta de Black Ops. 
La carpeta que necesitas seleccionar muy probablemente se llama `pluto_t5_full_game` o `Call of Duty Black Ops`.  
No selecciones la carpeta Games o tu carpeta Documentos. **Selecciona la carpeta que contiene los archivos de Black Ops!**
![BO1 in launcher](/images/docs/install/bo1-select-launcher.png)

Si estás usando una copia de Steam, el juego estará en la siguiente ruta: `C:\Program Files (x86)\Steam\steamapps\common\Call of Duty Black Ops`

Si usaste el torrent, el juego estará en una carpeta llamada `pluto_t5_full_game`

(Si alguna vez necesitas reseleccionar la carpeta del juego, simplemente dale click al ícono de la tuerca al lado del botón que dice PLAY)

---

### Error de T5: Invalid Game Path (Ruta de juego inválida)

Como dice el error, seleccionaste una ruta inválida para tu juego, por lo que esta no contiene los archivos del juego.

![Invalid Game Directory](/images/docs/install/vlwamKe.png)

Si salta este error, significa que seleccionaste tu disco en vez de la carpeta del juego. 
`C:\` no es la carpeta de Black Ops 1. 

![img](/images/docs/install/error-401.png)

En ambos casos, la manera de arreglar este error es darle clic en Game settings (Configuración de juego) en el iniciador y seleccionar la carpeta que contiene los archivos de Black Ops.
Si no puedes encontrarla, entonces lee la [guía desde el comienzo](#t5-black-ops-1) de nuevo.

![img](/images/docs/install/MnkAcr8.png)

---

**¡Felicitaciones! Completaste la guía de instalación.**

Para ejecutar Black Ops, simplemente abre el iniciador de Plutonium y dale clic en PLAY.

## Guitar Hero III

Esta sección cubrirá la instalación de Guitar Hero III.

1. Descarga [PreLoader.exe](https://plutonium.pw/III/PreLoader.exe) y guárdalo en una carpeta vacía. PreLoader descargará los archivos del juego en esta carpeta.

2. Ejecuta PreLoader.exe y deja que termine de descargar y configurarse.

3. Ejecuta GH3.exe para iniciar el juego.

4. Si el juego te pregunta si quieres jugar online, confírmalo. Luego escoge Crear una cuenta nueva.

5. Crea una cuenta nueva usando el usuario y contraseña de tu elección (**El nombre solo puede contener minúsculas**) y deja el campo de "License" (Licencia) vacío.

<Alert variant="warning">

No inicies sesión con tu cuenta del foro de Plutonium, las cuentas para este juego no están vinculadas al foro.

</Alert>

**Eso es todo, ¡diviértete jugando!**
