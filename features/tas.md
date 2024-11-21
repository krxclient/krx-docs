---
icon: stopwatch
---

# TAS (Speedrun Asistido por Herramientas) ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)

La pestaña **TAS** en la versión Ultimate del cliente KRX es una función en beta diseñada para un juego asistido por herramientas avanzadas, permitiendo entradas precisas y repetibles.  
Para una experiencia TAS más fluida, recomendamos usar el comando `/showall` al ingresar a un servidor.  
*Nota: Esta función está en proceso de rediseño, y su funcionalidad podría cambiar en el futuro.*

---

## **Captura de pantalla**
![Menú TAS](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/tas-menu.png)

---

## **TAS**
- **Habilitar**: Activa TAS y te teletransporta al mundo TAS.  
- **TPS (Ticks Por Segundo)**: Ajusta la velocidad de ticks para las entradas asistidas (TPS predeterminado para Teeworlds: 50).  
- **Reproducción de Dummy**: Habilita el soporte de dummies en modo TAS.  
- **Predicción de Jugadores**: Añade otros jugadores al mundo TAS.  
- **Ignorar Advertencias Iniciales**: Suprime mensajes de advertencia al inicio del TAS.  
- **Detener Ratón al Pausar**: Desactiva el ratón cuando TAS está pausado, permitiendo jugadas legítimas.  
- **Usar Entrada de Rebobinado**: Configura la entrada del ratón para coincidir con la entrada rebobinada, creando repeticiones más realistas.  
- **Mostrar Puntería Real**: Muestra la dirección de puntería real durante la repetición TAS.

---

## **Herramientas**
- **Rebobinado Automático**: Rebobina automáticamente hasta el último tick seguro antes de congelarse.  
- **Avance Automático**: Avanza automáticamente al primer tick antes de descongelarse.  
- **Ticks de Rebobinado**: Establece el número de ticks a rebobinar (predeterminado: 1 tick).  
- **Ticks de Avance**: Establece el número de ticks a avanzar (predeterminado: 1 tick).  
- **Pausar**: Pausa TAS después de rebobinar o avanzar automáticamente.  
- **Paso**: Rebobina o avanza exactamente un tick, permitiendo movimientos precisos en cada tick.

---

## **Puntería Falsa**
- **Habilitar**: Activa el modo de puntería falsa para desviar objetivos.  
- **Modo**: Selecciona el tipo de puntería falsa (por ejemplo, Puntería Robot).

---

## **Reproducción Automática**
- **Habilitar**: Carga y reinicia automáticamente las repeticiones.  
- **Reiniciar al Congelarse**: Reinicia la repetición al ocurrir una congelación.  
- **Matar al Reiniciar**: Mata al jugador cuando termina la repetición.

---

## **Modo Dios**
- **Super**: Activa el comando RCON `super` en el mundo TAS.  
- **Arma**: Permite darte un arma (excepto Ninja, debido a problemas conocidos).  
- **Dar Arma**: Otorga el arma seleccionada.

---

## **Atajos de Teclado**
- **Habilitar TAS**: Asigna una tecla para activar TAS.  
- **Grabar Repetición**: Asigna una tecla para iniciar la grabación de una repetición.  
- **Cargar Repetición**: Asigna una tecla para cargar una repetición.  
- **Reaparecer en TAS**: Asigna una tecla para reaparecer en modo TAS.  
- **Pausar TAS**: Asigna una tecla para pausar TAS.  
- **Rebobinar TAS**: Asigna una tecla para rebobinar durante TAS.  
- **Avanzar TAS**: Asigna una tecla para avanzar durante TAS.

---

## **Opciones Adicionales**
- **Carpeta de Repeticiones**: Abre la carpeta donde se almacenan las repeticiones TAS.  
- **Cargar/Guardar**: Carga o guarda repeticiones.  
- **Continuar**: Reanuda la reproducción desde el último tick de una repetición seleccionada.  
- **Campo de Nombre Personalizado**: Guarda repeticiones con un nombre personalizado (por ejemplo, `mi_tas`).  

---

## **Preguntas Frecuentes**
1. **P: ¿Por qué no veo armas en TAS?**  
   **R:** No ejecutaste el comando `/showall`.  

2. **P: ¿Por qué no puedo continuar mi run tras un cambio de mapa?**  
   **R:** Continuar no está soportado entre cambios de mapa. Detén la grabación, únete al mapa en otro servidor y continúa desde ahí.  

3. **P: ¿Qué significan estas advertencias como `Verify TAS Integrity failed...`?**  
   **R:** Estas advertencias garantizan runs TAS fluidos. Puedes ignorarlas en su mayoría, pero ayudan a depurar problemas. Compártenos las advertencias si encuentras inconvenientes.  

4. **P: ¿Por qué falló mi TAS en medio de un run?**  
   **R:** Los fallos de TAS suelen deberse al lag. Usa la configuración apropiada de `cl_prediction_margin` y reinicia la repetición desde la posición inicial correcta. Contacta soporte si el problema persiste.  

5. **P: ¿Por qué no puedo moverme en TAS?**  
   **R:** Es probable que TAS esté pausado o `krx_tasrespawn` esté configurado en 1. Despausa TAS o ejecuta `krx_tasrespawn 0` en la consola para solucionarlo.  

6. **P: ¿Por qué no veo nada al entrar en TAS?**  
   **R:** Necesitas reaparecer. Usa el atajo de Reaparecer para resolverlo.  

7. **P: ¿Por qué no puedo rebobinar o avanzar?**  
   **R:** Debes empezar a grabar en TAS para usar rebobinado o avance. Si tienes rebobinado/avance por pasos habilitado, los cambios podrían ser demasiado sutiles para notarse; desactívalo si es necesario.  
