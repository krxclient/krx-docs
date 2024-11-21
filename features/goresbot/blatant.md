---
icon: fire
---

# Blatant ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
El **Blatant** Gores bot en KRX Client está diseñado para ayudarte a enfrentar mapas de Gores de todo tipo, desde fáciles hasta extremos.  
*Nota: Al usar bots de evitación, por favor ajusta un mayor `cl_prediction_margin`, consulta [configuración](../settings.md) y elige el margen de predicción según tu ping.*

---

## **Captura de pantalla**
![Blatant Menu - Recommended Settings](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/blatant-menu.png)

---

## **Evitación**
- **Enable**: Activa la funcionalidad de evitar.
- **Player Prediction**: Predice los movimientos de otros jugadores.
- **NSIF**: Una característica avanzada que rastrea las secuencias de entrada previas y cambia a NSIF cuando la entrada actual de Blatant no persiste lo suficiente.
- **Afk Protection**: Desactiva automáticamente el Gores bot cuando se detecta que el usuario está AFK después del tiempo especificado de **Afk Time**.
  - **Afk Time**: Configurable en segundos.

## **Configuración**
- **Hook Assistance**: Activa las entradas de gancho para el Gores bot.
- **Direction Assistance**: Habilita la entrada direccional para el Gores bot.
- **Check Ticks**: Especifica cuántos ticks en el futuro el Blatant escanea para predecir.
- **Kick in Ticks**: Determina la duración mínima de la entrada actual para que Blatant no se active.
- **Action Ticks**: Similar a Check Ticks, pero se aplica a las acciones individuales durante los escaneos de Blatant.

## **Limitación de Tasa**
- **Enable**: Habilita la limitación de tasa para varias acciones.
- **Hook/Unhook**: Limita la frecuencia de acciones de gancho y desenganche.
- **Direction/No Direction**: Controla la limitación de tasa relacionada con la dirección.
- **Hook Check**: Aplica límites de dirección solo cuando no se está enganchando.
  - **Hook Ticks**: Establece la duración de la limitación de tasa de gancho en ticks.
  - **Unhook Ticks**: Define la duración de la limitación de tasa de desenganche en ticks.
  - **Move Ticks**: Configura la duración de la limitación de tasa para movimiento direccional.
  - **Stand Ticks**: Ajusta la duración de la limitación de tasa para acciones estáticas.

## **Varios**
- **Drag Support**: Proporciona datos adicionales al aimbot, ayudando a evitar direcciones que puedan llevar al congelamiento de tu personaje.
- **Track Point**: Rastrea la dirección actual y, si es posible enganchar, la sigue durante toda la duración del escaneo.
- **Rehook Action**: Considera escenarios de reenganche en el escaneo de Blatant.
- **Safe Aim Tracking**: Asegura el rastreo solo si la dirección rastreada permanece válida durante toda la duración del escaneo.
- **Tile Distance**: Ajusta el tamaño de los azulejos evitados, diseñado para hacer que las acciones de Blatant parezcan más legítimas.

## **Azulejos**
- **Teles**: Evita los azulejos de teletransportación.
- **Unfreeze**: Evita los azulejos de descongelación.
  - **Ticks**: Duración configurable de comprobación para los azulejos de descongelación.
- **Death**: Evita los azulejos de muerte.

## **Aimbot**
- **Enable**: Activa el aimbot de evitación.
- **Auto Aim**: Escanea todas las direcciones y selecciona la más viable.
- **Aim Assist**: Apunta a la dirección más cercana al ratón que permanece válida por más tiempo.
- **Upward Aim**: Prioriza las direcciones hacia arriba que persisten por más tiempo.
- **Points**: Especifica el número de puntos a evaluar por segmento.
- **Segments**: Define la cantidad de segmentos a escanear.
- **FOV**: Campo de visión configurable para el objetivo.
- **Check Ticks**: Ajusta la duración de los escaneos para los cálculos del aimbot.

## **Visuales**
- **Track Point**: Muestra visualmente los puntos rastreados.
- **Aimbot**: Destaca los puntos objetivo del aimbot.
- **Path**: Muestra la ruta actual seguida por el bot.

## **Configuración**
Configurar este bot no es trivial, debes experimentar con cada una de estas configuraciones. Aquí tienes una configuración básica para comenzar:
- **NSIF**: ENCENDIDO
- **Hook Assistance**: ENCENDIDO
- **Direction Assistance**: ENCENDIDO
- **Check Ticks**: 26
- **Kick in Ticks**: 20
- **Action Ticks**: 26
- **Drag Support**: ENCENDIDO
- **Track Point**: ENCENDIDO
- **Rehook Action**: ENCENDIDO
- **Safe Aim Tracking**: ENCENDIDO para máxima seguridad, si no, APAGADO
