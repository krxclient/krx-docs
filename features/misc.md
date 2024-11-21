---
icon: sparkles
---

# Misceláneo

La pestaña **Misc** en el cliente KRX ofrece una variedad de herramientas y funciones diseñadas para mejorar la jugabilidad, brindar protecciones y habilitar mecánicas de trolleo divertidas.

---

## **Captura de pantalla**
![Menú Misc](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/misc-menu.png)

---

## **Características**

### **Bots**
- **Moonwalk**: Hace que el jugador realice un "moonwalk" al presionar las teclas izquierda y derecha, alternando la dirección del movimiento.  
- **Auto Fire**: Dispara automáticamente tu arma cuando mantienes presionado el botón de disparo.  
- **Auto Rehook**: Después de enganchar con éxito a un jugador, si mantienes presionado el botón de hook, intenta automáticamente volver a engancharlo.  
- **Auto Jump Save**: Salta automáticamente para evitar caer en zonas de freeze.  
- **Quick Stop**: Detiene al jugador rápida y suavemente ajustando la dirección del movimiento para contrarrestar su velocidad actual.  
- **Avoid Freeze**: Ayuda a evitar zonas de freeze usando movimientos hacia la izquierda o derecha.  
- **Dummy Fly**: Tu dummy realiza automáticamente hook fly contigo, haciendo que el dummy utilice hammer y hook también. ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  
- **Jet Ride**: Funciona como el hook ride bot pero con un jetpack. Se controla con A/W/S/D. ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  
- **Auto Aled**: Realiza hammer automáticamente cuando es posible un "aled". ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  

### **Protecciones**
- **Random Timeout Seed**: Genera una nueva semilla de timeout antes de conectarse a un servidor para evitar el rastreo. Nota: No podrás reincorporarte a tu posición anterior después de un timeout con esta función habilitada.
- **Version Spoofer**: Falsifica la versión/ID del cliente para evitar restricciones. Si tienes dudas, déjalo desactivado.

### **Mod Detector**  
- **Enable**: Activa la función Mod Detector para identificar posibles moderadores o jugadores sospechosos en el servidor.  
- **Detect by Names**: Escanea los nombres de los jugadores en busca de moderadores conocidos.  
- **Detect Suspicious Players**: Escanea los nombres de los jugadores para detectar moderadores potenciales o jugadores que podrían reportarte.  
- **Leave on Mod Detection**: Se desconecta automáticamente del servidor si se detecta un moderador potencial.  
- **Leave on Warn Detected**: Se desconecta automáticamente si se detecta un moderador o jugador que podría reportarte.  

### **Auto Unfreeze** ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)
- **Enable**: Activa la función Auto Unfreeze, que dispara automáticamente un láser hacia una pared para descongelarte al atravesar zonas de freeze.
- **Advanced Settings**: Habilita opciones de configuración detalladas para un control más preciso.
    - **Bounces**: Determina cómo rebota el láser en las paredes:
        - **Least**: Selecciona una dirección con la menor cantidad de rebotes, garantizando una descongelación más rápida.
        - **Most**: Selecciona una dirección con la mayor cantidad de rebotes. Útil en escenarios TAS, ya que más rebotes resultan en tiempos de recarga más rápidos.
    - **Silent**: Hace que los ajustes de puntería sean invisibles en tu pantalla pero visibles para otros.
    - **Points**: Configura la cantidad de puntos considerados al verificar direcciones para descongelar. Valores más altos proporcionan verificaciones más precisas.
    - **Current Dir Ticks**: Establece cuántos ticks del láser se utilizan para calcular la dirección actual. Ajusta para mayor precisión.
    - **Ticks**: Define cuántos ticks del láser se analizan al determinar la mejor dirección para descongelar.
    - **FOV**: Ajusta el campo de visión para determinar el rango de puntería del láser.

### **Fake Aim**
- **Enable**: Activa el comportamiento de fake aim para confundir o despistar a otros jugadores.
- **Send Always**: Si está activado, la dirección del aim se enviará al servidor cada tick (se verá más suave para otros).
- **Visible**: Muestra el fake aim en tu pantalla.
- **Modes**: Determina cómo se comporta el fake aim:
  - **Mouse Pos**: Ajusta tu puntería para seguir la posición del mouse, haciendo que el aimbot del gores bot parezca menos obvio.
  - **Robot Aim**: Actualiza tu posición de puntería solo al enganchar o disparar.
  - **Spinbot**: Rota rápidamente tu puntería en un movimiento giratorio.
  - **Random**: Mueve tu puntería en direcciones aleatorias.
  - **Fake Angles**: Apunta en la dirección opuesta a tu cursor.
  - **Aimbot Troll Aim**: Apunta siempre al jugador más cercano.

### **Otros**
- **Change Name on Finish**: Cambia automáticamente tu nombre justo antes de cruzar la línea de meta.
- **Auto Team**: Se une automáticamente al equipo seleccionado y lo bloquea.
- **Anti AFK**: Evita que se te marque como AFK.
- **Kill on Freeze**: Mata automáticamente a tu personaje al quedar congelado.
- **Fast Input**: Hace que tus entradas parezcan 1 tick más rápidas (20ms), aunque solo es un efecto visual.
- **Ignore Replay Warnings**: Suprime mensajes de advertencia relacionados con replays TAS.
- **Hide Chat Bubble**: Oculta la burbuja de chat para que otros jugadores no sepan cuándo estás escribiendo.
- **Auto Verify**: Verifica automáticamente en servidores protegidos como `ger10.ddnet.tw`.
- **Send Occasional Ads**: Envía anuncios ocasionales en el chat.

### **Troll**
- **Emote Spam**: Envía emotes aleatorios lo más rápido posible.
- **Killsay/Deathsays**: Envía mensajes predefinidos al matar o morir.
- **Fancy Chat Font**: Cambia la fuente del chat para una apariencia única.
- **Mass Mention Spam**: Menciona a múltiples jugadores repetidamente.
- **Chat Repeater**: Repite automáticamente el mensaje de chat de otro jugador alternando entre mayúsculas y minúsculas (por ejemplo, "MeSsAgE").

### **ID Stealer**
- **Enable**: Activa la función ID Stealer, permitiéndote copiar la información de otro jugador.
- **Closest Player**: Si está activado, apunta al jugador más cercano para copiar sus detalles. Si está desactivado, selecciona un jugador aleatorio en el servidor.
- **Steal Name**: Copia el nombre del jugador objetivo.
- **Steal Clan**: Copia el nombre del clan del jugador objetivo.
- **Steal Skin**: Copia la skin del jugador objetivo.
- **Steal Flag**: Copia la bandera del país del jugador objetivo.
- **Steal Eye Emote**: Copia la expresión facial del emote de ojos del jugador objetivo.
- **Stealer Speed**: Ajusta el intervalo (en segundos) para actualizar los detalles robados.

### **Silent Walk**
- **Enable**: Activa la función Silent Walk, que oculta ciertos indicadores para hacer tus acciones menos notorias.
- **Direction**: Oculta las flechas direccionales que muestran tu movimiento.
- **Jump**: Oculta la flecha de salto, dificultando que otros vean cuándo estás saltando.
- **Hook**: Envía un hook invisible en la dirección de tu puntería. Ten en cuenta que el alcance del hook es limitado.
- **Hook Closest**: Envía un hook invisible al jugador más cercano. Ten en cuenta que el alcance del hook es limitado.

---

## **Configuración**

Para la mayoría de los casos, vale la pena habilitar las siguientes funciones:
- **Auto Fire**: Dispara automáticamente tu arma, facilitando enfocarte en apuntar y moverte.
- **Avoid Freeze**: Especialmente útil en mapas gores, esta función te ayuda a evitar zonas de freeze.
- **Quick Stop**: Ideal para mapas de bloques, te ayuda a detenerte rápida y precisamente.
- **Auto Jump Save**: Función situacional para evitar caer en freeze; actívala según sea necesario.
- **Mod Detector**: Úsalo si te preocupa que te observen o te baneen moderadores.
- **Fast Input**: Muchos usuarios dicen que mejora la sensación de respuesta; pruébalo.
- **Auto Verify**: Una función de calidad de vida que automatiza la verificación en servidores protegidos por DDOS. Vale la pena mantenerla activada para mayor comodidad.

Ajusta estas funciones según tus necesidades de juego específicas y experimenta para encontrar la mejor combinación para tu estilo.
