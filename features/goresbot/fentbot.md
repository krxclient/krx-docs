---
icon: robot
---

# Fent Bot ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
La pestaña **Fent Bot** en KRX Client ofrece una herramienta avanzada para automatizar mediante búsqueda de caminos y túneles.  
*Nota: Al usar bots de evitación, por favor utiliza un `cl_prediction_margin` más alto. Consulta [configuración](../settings.md) y elige el margen de predicción según tu ping.*

---

## **Captura de pantalla**
![Fent Bot Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/fentbot-menu.png)

---

## **Evitación**
- **Player Prediction**: Habilita la predicción de los movimientos de otros jugadores.
- **Advanced Settings**: Desbloquea opciones avanzadas de personalización para el comportamiento del bot.
- **Use Skibidiforce**: Activa el algoritmo Skibidiforce para una búsqueda de caminos avanzada.
  - **Skibidiforce Depth**: Configura la profundidad de los cálculos de Skibidiforce.
- **Fent Ticks**: Define la duración del tick para la búsqueda de caminos basada en fent.
- **Tweaker Inputs**: Número de entradas de tweaker.
- **Tweaker Ticks**: Ajusta la duración del tick para las entradas de tweaker.
- **Inject Fent**: Una acción de un solo clic para comenzar el escaneo.

## **Varios**
- **Skibidiforce Aim Points**: Configura el número de puntos de apunte utilizados por Skibidiforce.
- **Render Path**: Muestra visualmente el camino calculado.
- **Render Tunnels**: Destaca los túneles utilizados para la búsqueda de caminos.
- **Spectate Scan**: Permite observar el progreso del escaneo durante el proceso de escaneo.
- **Tunnel Editor**: Proporciona una interfaz para personalizar túneles manualmente.
- **Auto Tunnels**: Genera automáticamente túneles para movimiento optimizado desde un replay cargado.
- **Tunnel Width**: Ajusta el ancho de los túneles generados automáticamente.
- **Clear Tunnels**: Elimina todos los túneles.

---

## **Configuración**
- En la mayoría de los casos, usar la configuración predeterminada proporcionada por KRX es suficiente. Aquí tienes una configuración posible para usuarios más avanzados con buenos CPUs:
- **Player Prediction**: OFF
- **Advanced Settings**: ON
- **Use Skibidiforce**: ON
- **Skibidiforce Depth**: 4
- **Fent Ticks**: 1000
- **Tweaker Inputs**: máximo
- **Tweaker Ticks**: 4-8
