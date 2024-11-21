---
icon: gear
---

# Configuración

La pestaña **Configuración** en el cliente KRX te permite asignar atajos de teclado y ajustar características específicas para mejorar tu experiencia de juego.

---

## **Captura de pantalla**
![Menú de Configuración](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/settings-menu.png)

---

## **Atajos de teclado**
- **Aimbot**: Activa/desactiva el aimbot.  
- **Aimbot Auto Hook**: Lanza automáticamente el gancho a objetivos cuando el Aimbot está habilitado.  
- **Aimbot Auto Shoot**: Dispara automáticamente a objetivos cuando el Aimbot está habilitado.  
- **Balance Bot**: Activa el bot para mantener el equilibrio en los tees.  
- **Emote Spam**: Permite el envío continuo de emoticonos.  
- **Hook Spam**: Habilita el envío rápido de ganchos.  
- **Super DynCam**: Permite un zoom ilimitado con la cámara dinámica.  
- **Pixel Walk**: Permite movimientos precisos, píxel por píxel, al usar teclas direccionales.  
- **Hook Nearest Collision**: Automáticamente lanza el gancho a la colisión más cercana.  
- **Quick Stop**: Detiene instantáneamente el movimiento al soltar las teclas direccionales, permitiendo frenar lo más rápido posible.  
- **Hook Ride (arriesgado)**: Activa el bot de Hook Ride.  
- **Record Replay**: Comienza a grabar las entradas del jugador.  
- **Load Replay**: Carga entradas previamente grabadas.  
- **Avoid Freeze**: Activa el bot para evitar tiles de freeze.  
- **Auto Edge**: Activa el bot para aterrizar automáticamente en los bordes cercanos a tiles de freeze, muerte o teletransporte. ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  
- **Laser Unfreeze Bot**: Activa un bot para descongelarte automáticamente usando el láser. ![Premium](https://img.shields.io/badge/Premium-%23ffba00?style=flat-square)  
- **Avoid Auto Drag**: Automáticamente engancha al tee más cercano sin congelarse cuando esta función está activa. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)  
- **Avoid Track Points**: Activa el seguimiento avanzado de puntos para el Blatant Gores Bot. Consulta [Blatant Gores Bot](blatant.md) para más detalles. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)  

---

## **Ajustes**
- **Teleport Prediction**: Habilita la predicción de teletransportes para TAS o Gores Bot; de lo contrario, los teletransportes se reemplazan con freeze. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)  
- **Advanced Settings**: Desbloquea configuraciones avanzadas para optimizar todos los bots KRX al máximo: ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
   - **Death Tile Prediction**: Predice tiles de muerte para los bots, incluyendo TAS y Gores Bot. De lo contrario, los tiles de muerte se ignoran.  
   - **Move Restrictions Prediction**: Predice "air stoppers". Desactivar esta opción puede mejorar significativamente el rendimiento del bot.  
   - **Player Loop**: Predice colisiones entre tees. Desactivar solo elimina el manejo de colisiones, lo que puede mejorar significativamente el rendimiento.  
   - **Prediction Margin**: Ajusta el margen de predicción. Valores más altos te hacen menos vulnerable a picos de lag, pero podrían hacer que otros jugadores parezcan con más lag.
- **Balance Bot Offset**: Configura la agresividad del bot para mantener el equilibrio. Valores más altos reducen las correcciones de movimiento.  
- **Hook Nearest FOV**: Ajusta el campo de visión para la función **Hook Nearest Collision**.  

---

## **Configuración**

1. Abre la pestaña **Configuración** en el cliente KRX.  
2. Asigna atajos personalizados según tus preferencias.  
3. Ajusta los ajustes para adaptarlos a tus necesidades de juego. A continuación, te recomendamos algunas configuraciones:  
   - **Teleport Prediction**: Se recomienda mantener deshabilitada a menos que uses TAS. No actives esta opción al usar el Gores Bot. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)  
   - **Advanced Settings**: Se recomienda mantener deshabilitada a menos que sepas lo que estás haciendo. ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)  
      - **Death Tile Prediction**: Se recomienda deshabilitada ya que ralentiza los bots, aunque es útil para TAS.  
      - **Move Restrictions Prediction**: Recomendado habilitar para un juego casual. Desactivar para mejorar el rendimiento en bots.  
      - **Player Loop**: Recomendado habilitar para un juego casual. Desactivar para mejorar el rendimiento en bots.  
      - **Prediction Margin**: Ajusta según tu ping (por ejemplo, para 50ms de ping, configúralo en ~50). Valores mayores a 20 se recomiendan para evitar problemas con el bot.
   - **Balance Bot Offset**: Valor recomendado: ~2.  
   - **Hook Nearest FOV**: Recomendado un FOV más bajo (por ejemplo, 30) para reducir el lag en CPUs de bajo rendimiento.  
