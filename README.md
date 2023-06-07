# Manejo de Interrupciones 
En esta practica se diseñara un contador binario de 10 bits simulandolo con 10 leds, el contador aumentara 1 bit cada segundo a este circuito se conectaran 2 botones, el boton A tendra la funcion de cambiar el contador de manera descendente a ascendente, y el segundo boton B cambiara la velocidad del contador x2, x4, x8, x1.  En un procesador ARM Cortex-M3

Para que esta practica pueda funcionar correctamente se tiene que Configurar el reloj del sistema (SysTick) para generar una excepción, y Configurar una interrupción externa (EXTI).

### Configuracion "SysTick"
En el archivo "SysTick_isr.s" es la configuración y el manejo de la interrupción generada por el temporizador SysTick.
En donde primero se inicializa una interrupcion y despues se ejecuta cada vez que se produce una interrupcion.

### Configuracion "exti_isr.s"
En este archivo se implementa rutinas de interrupción para los eventos EXTI0 y EXTI4. 

### Compilacion del proyecto
Utilizaremos los comandos make, make write, make clean

    make          se usa para ensamblar (crear el binario   .bin)
    make write    se usa para escribir en el microcontrolador(grabar)
    make clean    se usa para limpiar los archivos binarios .o  .bin 

## Diagrama de Hardware 
![lab6](https://github.com/Miguel-Rosario/prueba/assets/126648916/f3e39fec-8b3a-40a1-a48a-d640cd2c53fa)
