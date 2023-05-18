# Juegos personalizados / Jugar con amigos

<Alert variant="tip">

En T6 y T5, la mayoría de los jugadores deberían poder invitar a personas directamente.  
En caso de que no funcione, deberás seguir pasos adicionales, como antes.  
En T4 e IW5, es posible que debas seguir pasos adicionales para poder unirte a tus amigos.  

Si no sabes a qué se refieren estos nombres de código, puedes consultar el [documento de explicaciones del motor](https://plutonium.pw/docs/engine-explanations/).

</Alert>

Esta guía te enseñará cómo jugar con amigos a través de Internet en una partida de juegos personalizados.  
No importa qué juego estés intentando jugar, **el primer paso es seguirse mutuamente en el foro**.  
Consulta [Agregar un amigo a tu lista de amigos](#añadir-a-un-amigo-a-tu-lista-de-amigos).

El alojamiento no es complicado, pero implica varios conceptos de redes que debes entender antes de comenzar, así que asegúrate de tomarte tu tiempo para leer esta guía y comprender los conceptos involucrados en el alojamiento.  
También puedes consultar la [Introducción](#introducción) si hay algo que no entiendes.

## Introducción

### ¿Por qué necesito hacer todo esto?

En primer lugar, debes saber que Plutonium te solicita que sigas todos estos pasos porque alojar servidores cuesta dinero, por eso la mayoría de los juegos en Steam no requieren más que hacer clic en "Crear un juego".  
Pero para juegos independientes y proyectos apasionados como Plutonium, alojar un servidor para todos costaría demasiado dinero, por lo que debes alojar tus propios juegos, lo cual es gratuito para todos.  
En cuanto a Black Ops y Black Ops II, Plutonium trabajó en un sistema que intenta hacer que todo funcione directamente, pero dependiendo de la configuración de tu red, podría fallar y luego necesitarás redirigir puertos para asegurarte de que el sistema funcione.

### ¿Cómo funciona el alojamiento?

Básicamente, cuando deseas alojar un servicio, como un servidor de juegos (o un juego privado con tus amigos), hay un concepto importante que debes entender: quién puede acceder a mi red y a qué servicio pueden acceder. No quieres que las personas externas tengan acceso a todo en tu PC.
Si deseas jugar con 2 PC conectadas al mismo enrutador de Internet, puedes conectarte entre sí utilizando tu **IP local** porque ambos dispositivos confían el uno en el otro.
Pero cuando deseas jugar con personas que no están conectadas a tu enrutador (es decir, personas fuera de tu hogar), eso es diferente, ya que se consideran extrañas y posibles amenazas. Aquí es donde entra en juego el concepto de **puertos y redirección de puertos**.

### ¿Qué es UPnP?

A lo largo de esta guía verás mencionadas las palabras "redirección de puertos" y "UPnP". Para alojar un servidor o un juego personalizado, necesitas realizar una redirección de puertos que requiere una configuración manual en tu enrutador.
La idea detrás de [UPnP](https://es.wikipedia.org/wiki/Universal_Plug_and_Play) es permitir que tu enrutador abra y cierre automáticamente puertos a medida que abres y cierras servicios (como servidores de juegos) en tu PC, por lo que básicamente es una redirección de puertos automática y sencilla.
Ten en cuenta que UPnP y la redirección de puertos son dos cosas diferentes, por lo que **la redirección de puertos no habilitará UPnP**, pero tienen el mismo objetivo. UPnP es útil para hacer que las cosas funcionen de inmediato sin ninguna configuración, pero no funciona con todas las configuraciones de red. Si no funciona para ti, deberás realizar la redirección de puertos manualmente.

### ¿Qué es redirigir puertos?

Para simplificarlo, todo lo que está conectado a Internet y se ejecuta en tu PC utiliza un [puerto](https://es.wikipedia.org/wiki/Puerto_(inform%C3%A1tica)).
El tráfico de Internet que pasa por estos puertos puede ser **conexiones salientes** (por ejemplo, tú conectándote a Google o a un servidor de juegos), lo cual no requiere nada de tu parte, o **conexiones entrantes**, lo que significa que recibes conexiones desde el exterior (alojamiento).
En este último caso, necesitas **redirigir** el puerto utilizado por tu servicio (en este caso, tu servidor de juegos) para indicarle a tu enrutador que permita conexiones desde el exterior en ese puerto específico.
De lo contrario, por defecto y por motivos de seguridad, las conexiones entrantes en ese puerto estarán bloqueadas. Así que si entendiste esto correctamente: solo el anfitrión necesita tener un puerto abierto (o UPnP habilitado) en su enrutador. Las personas que se unen no necesitan hacer nada en su extremo, al igual que cuando te unes a un servidor público.

### ¿Cómo habilitar UPnP?

- Habilita UPnP en tu enrutador si aún no está habilitado.  
Dado que cada enrutador es diferente, no podemos hacer una guía para cada uno.  
Te recomendamos buscar "nombre de tu enrutador + habilitar UPnP" en Google o buscar en la configuración de tu enrutador.

- Ve a Configuración de Windows -> Red e Internet, luego haz clic en Propiedades debajo del nombre de tu red.

![img](/images/docs/custom-games/PnaSif4.png)

- Configura el Perfil de red como Privado

![img](/images/docs/custom-games/hC6G8QN.png)

- Reinicia el juego

### ¿Cómo redirigir puertos?

Para alojar una partida privada sin UPnP o cuando tus amigos no pueden unirse de forma automática, necesitas realizar una redirección de puertos (consulta [¿Qué es redirigir puertos?](#qué-es-redirigir-puertos)).  
Dado que cada enrutador es diferente, no podemos proporcionar una guía para cada uno. Te recomendamos buscar en Google/Youtube "nombre de tu enrutador + redirigir puertos" o "nombre de tu [ISP](https://es.wikipedia.org/wiki/Proveedor_de_servicios_de_Internet) + redirigir puertos".

Puedes crear una regla de rango de puertos, por ejemplo, del 1000 al 1005, lo cual abrirá todos los puertos del 1000 al 1005, incluyendo el 1000 y el 1005, o puedes crear una regla para cada puerto necesario, el resultado es el mismo.  
El valor/rango del puerto se indica en la sección correspondiente a tu juego. Cada juego puede tener un puerto diferente, así que lee la sección del juego que estás intentando jugar en esa página.  
Por ejemplo, `28960-28961` significa tanto el puerto `28960` como el puerto `28961`, o un rango de puertos desde `28960` hasta `28961`.  
Por otro lado, `3074` significa que solo tienes que abrir ese puerto específico.

Abrir un solo puerto debería verse algo así como la captura de pantalla que se muestra a continuación. 
Aquí tienes las cosas más comunes que debes saber. Es posible que no tengas todas estas configuraciones.

- El nombre de la regla puede ser cualquier cosa, se recomienda algo descriptivo como "Plutonium T6".
- El protocolo es UDP (También funciona con "Ambos", pero no es necesario).
- El puerto/valor a ingresar es el puerto indicado en la sección correspondiente a tu juego.
- Los valores de puerto externo e interno siempre deben ser iguales.
- El puerto de destino es el puerto para tu juego.
- El puerto de origen puede estar en blanco o ser un comodín o "todo" dependiendo de tu enrutador. Debes permitir cualquier/todo puerto de origen.

![img](/images/docs/custom-games/port_forward_example.png)

## Añadir a un amigo a tu lista de amigos

Tanto tú como tu amigo necesitan seguirse mutuamente en los foros de Plutonium para poder unirse:

- Ve a [https://forum.plutonium.pw/users](https://forum.plutonium.pw/users), asegúrate de haber iniciado sesión y luego busca el nombre de tu amigo en Plutonium.
- Ve a su perfil y haz clic en el botón verde "+" (más) para seguirlo.
  - Si hay un corazón, eso significa que ya lo estás siguiendo.

Una vez que ambos se sigan mutuamente, verás a tu amigo en la lista de amigos del juego (o en la pestaña de la lista de amigos de Plutonium overlay para T4).  
Si después de seguirse mutuamente no pueden verse en la lista de amigos del juego, simplemente reinicia el juego.

## T6

En T6, invitar a tu amigo debería funcionar sin problemas.

### **Invitar a tu(s) amigo(s)**

- Asegúrate de que la privacidad de tu grupo esté configurada como "abierta" (P).
- Asegúrate de que nada bloquee la conexión (el firewall de tu enrutador, el firewall de tu antivirus, si tienes alguno, etc.).
- Abre la lista de amigos (F).
- Invita a tu amigo(s).

![invitar jugadores](/images/docs/custom-games/t6-inviting-as-host.gif)

Tu amigo(s) ahora puede(n) aceptar la invitación.

![aceptar una invitación](/images/docs/custom-games/t6-joining-sesh.gif)

### **Si no funciona**

Primero, asegúrate de haber seguido los pasos correctamente.
A continuación, puedes intentar dejar que otro amigo te invite a ti/otros jugadores.

Si aún no funciona, sin importar lo que hagas, tendrás que redirigir el puerto `3074` (UDP) en tu enrutador (consulta [Cómo redirigir puertos](#cómo-redirigir-puertos)).
Una vez hecho esto, puedes reiniciar tu juego e invitar a tu amigo(s) nuevamente siguiendo las instrucciones anteriores.

## IW5

En IW5, no hay una forma fácil de saber si UPnP está habilitado, excepto probándolo.
No hay un sistema de grupos en Plutonium IW5, por lo que tu amigo(s) solo puede(n) unirse a ti mientras estés en el juego.

### **Si UPnP está habilitado**

Inicia una partida privada y haz que tu amigo se una a ti siguiendo estos pasos:
- Abre el menú de amigos (F)
- Haz doble clic en el nombre de tu amigo que está siendo el anfitrión

### **Si UPnP está deshabilitado / no funciona**

- Redirige el puerto `27016` (UDP) en tu enrutador (consulta [Cómo redirigir puertos](#cómo-redirigir-puertos)).
- [Agrega el puerto a la lista blanca en el firewall de Windows](https://www.tomshardware.com/news/how-to-open-firewall-ports-in-windows-10,36451.html).
- Asegúrate de que nada bloquee la conexión (el firewall de tu enrutador, el firewall de tu antivirus, si tienes alguno, etc.).
- Una vez que hayas realizado esos pasos, abre tu juego e inicia una partida privada. **(Los grupos no funcionarán)**.

- Tu amigo ahora debería poder unirse a ti siguiendo estos pasos:
  - Abre el menú de amigos (F)
  - Haz doble clic en el nombre de tu amigo que está siendo el anfitrión

## T4

<Alert variant="tip">

En Plutonium T4 no hay un sistema de grupos, por lo que tu amigo(s) solo puede(n) unirse a ti mientras estás en el juego (o después de que se haya cargado la pantalla de carga).

Para poder jugar con tus amigos en la ronda 1 de zombies, puedes hacer que el juego espere en la pantalla de carga hasta que se conecte cierta cantidad de jugadores usando el siguiente comando: `sp_minplayers 2`.
Este comando debe ingresarse en la [consola](/docs/opening-console/).
Reemplaza `2` por la cantidad de jugadores que deseas esperar antes de comenzar el juego.

</Alert>

Una vez que tú y tu amigo se sigan mutuamente, la persona que desee ser el anfitrión de la partida privada debe hacer lo siguiente:

- Abre el juego y la lista de servidores (F10 o tecla de inicio).
- Ve a la pestaña de red y verifica si UPnP está habilitado.

---

### **Si UPnP está habilitado**

- Inicia una partida privada.

Si la partida requiere 2 jugadores para comenzar, puedes forzar su inicio de todos modos utilizando el botón de juego en solitario.
No te preocupes, en realidad no será en solitario, iniciará una partida privada en línea a la que tus amigos pueden unirse.
Alternativamente, puedes usar el comando `xpartygo` para forzar el inicio de la partida.

- Una vez que se haya iniciado el juego, tu amigo debería poder unirse haciendo doble clic en tu nombre en la pestaña de la lista de amigos de la superposición de Plutonium.

Si no puedes hacer que funcione incluso con UPnP habilitado, entonces tendrás que realizar una redirección de puertos.
Para esto, lee [Si UPnP sigue deshabilitado o no puedes conectar a pesar de tenerlo habilitado](#si-upnp-continúa-desactivado-o-no-puedes-conectar-a-pesar-de-estar-habilitado).

---

### **Si UPnP está desactivado**

- Habilita UPnP (consulta [Cómo habilitar UPnP](#cómo-habilitar-upnp))

- Si UPnP está habilitado, sigue las [instrucciones anteriores](#si-upnp-está-habilitado).
  Si no lo está, sigue las [instrucciones a continuación](#si-upnp-continúa-desactivado-o-no-puedes-conectar-a-pesar-de-estar-habilitado).

---

### **Si UPnP continúa desactivado o no puedes conectar a pesar de estar habilitado**

- Abre los siguientes puertos en tu enrutador: `28960-28961` (UDP) (Consulta [Cómo redirigir puertos](#cómo-redirigir-puertos))
- [Añade estos puertos a la lista blanca del firewall de Windows](https://www.tomshardware.com/news/how-to-open-firewall-ports-in-windows-10,36451.html)
- Asegúrate de que nada bloquee la conexión (el firewall de tu enrutador, el firewall del antivirus, etc.)
- Una vez completados estos pasos, abre el juego y comienza una partida privada. **(Las partidas en grupo no funcionarán)**

Si el juego requiere 2 jugadores para empezar, puedes forzar el inicio al iniciar una partida usando el botón "solo".  
No te preocupes, en realidad no es una partida en solitario, comenzará una partida privada en línea a la que tus amigos pueden unirse.  
Alternativamente, puedes usar el comando `xpartygo` para forzar el inicio de la partida.

- Tu amigo debería poder unirse ahora haciendo doble clic en tu nombre en la pestaña "Friends List" de la superposición de Plutonium.

## T5

- Asegúrate de que la privacidad de tu grupo esté configurada como "abierta", "solo amigos" o "solo invitados".
- Asegúrate de que nada bloquee la conexión (el firewall de tu enrutador, el firewall del antivirus, etc.)
- Abre la lista de amigos.
- Invita a tu amigo/amigos.

### Multijugador

Para jugar con amigos en T5 Multijugador, debes comenzar una partida privada e invitar a tus amigos a unirse.  
Debes estar dentro del juego para unirte. Invitar a tus amigos en un lobby multijugador no funcionará.

![imagen invitando a un amigo a unirse](/images/docs/custom-games/t5-invite.png)

![imagen de un amigo dentro del juego](/images/docs/custom-games/t5-mp-joined.png)

### Zombies

Para jugar con amigos en T5 Zombies, puedes invitarlos mientras estás en un lobby.

![imagen en el lobby invitando a un amigo](/images/docs/custom-games/t5-zm-invite.png)

![imagen del amigo dentro del lobby](/images/docs/custom-games/t5-zm-joined.png)

### **Si no funciona**

Asegúrate de haber seguido los pasos correctamente.  
Luego, puedes intentar que otro amigo te invite a ti/los otros jugadores.

Si aún no funciona, sin importar lo que hagas, entonces tendrás que redirigir el puerto `3074` (UDP) en tu enrutador (consulta [Cómo realizar la redirección de puertos](#cómo-redirigir-puertos)).
Una vez hecho esto, puedes reiniciar tu juego e invitar a tus amigo(s) nuevamente siguiendo las instrucciones anteriores.

## Notas adicionales

### Juego en LAN

Si tú y algunos o todos tus amigos están en la misma red local (LAN), se pueden conectar a través de la IP interna. Si todos los jugadores están en la misma LAN, no es necesario realizar redirección de puertos.

Si quieres encontrar tu IP interna, abre una ventana de símbolo del sistema (Command Prompt) y escribe `ipconfig`.

![img](/images/docs/custom-games/gUXeTOE.png)

Tu IP local estará bajo `Dirección IPv4`.

A partir de ahí, cada cliente en tu LAN simplemente podrá conectarse [abriendo la consola](/docs/opening-console/) y ejecutando

```cs
connect AquíColocaLaDirecciónIPv4DelAnfitrión
```

### Conexión a través de una dirección IP

Si la lista de amigos no funciona para ti, puedes intentar conectarte a través de una dirección IP.

Haz que el anfitrión obtenga su dirección IP (puede hacerlo a través de la pestaña de Red del Overlay de Plutonium o mediante [WhatIsMyIP](https://www.whatismyip.com/))

Luego, simplemente podrás conectarte [abriendo la consola](/docs/opening-console/) y ejecutando el siguiente comando:

```cs
connect AquíColocaLaDirecciónIPDelAnfitrión
```
