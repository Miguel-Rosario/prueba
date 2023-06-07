# Manejo de Interrupciones 
En esta practica se diseñara un contador binario de 10 bits simulandolo con 10 leds, el contador aumentara 1 bit cada segundo a este circuito se conectaran 2 botones, el boton A tendra la funcion de cambiar el contador de manera descendente a ascendente, y el segundo boton B cambiara la velocidad del contador x2, x4, x8, x1.  En un procesador ARM Cortex-M3

Para que esta practica pueda funcionar correctamente se tiene que Configurar el reloj del sistema (SysTick) para generar una excepción, y Configurar una interrupción externa (EXTI).

### Configuracion "SysTick"
En el archivo "SysTick_isr.s" es la configuración y el manejo de la interrupción generada por el temporizador SysTick.
En donde primero se inicializa una interrupcion y despues se ejecuta cada vez que se produce una interrupcion.

### Configuracion "exti_isr.s"
En este archivo se implementa rutinas de interrupción para los eventos EXTI0 y EXTI4. 


## Diagrama de Hardware 
![arm4 drawio (5)](https://github.com/Miguel-Rosario/prueba/assets/126648916/b9435be1-33c5-4e44-a88a-ce83cb1022f4)
