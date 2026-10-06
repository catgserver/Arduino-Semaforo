# Arduino-Semaforo
Replicaremos el funcionamiento de un semáforo utilizando placa Arduino R4 y el software Arduino IDE para programar el microcontrolador.

## Herramientas y/o piezas que necesitamos:
- 1x placa Arduino
- 3x Diodos LED (Rojo, Amarillo y Verde)
- 3x Resistencia de 220 Ohm
- 1x Protoboard
- Cables de conexión tipo jumper (Macho-Macho)

## Proceso
Primero vamos a elegir que pines de salida se usará de la placa de Arduino para activas 3 lineas del protoboard, en esas lineas estarán conectadas los Leds verde, amarillo y rojo.
En cada LED conectaremos en la linea del positvo su respectiva resistencia y por consiguiente a salida a tierra y vinculada a Ground del Arduino.
Después de tener listo el circuito armado para la prueba procederemos a escribir el código en Arduino IDE.

## Codigo para IDE

```
const int rojo = 8;
const int amarillo = 9;
cons tint verde = 10;

void setup()[
pinMode(rojo, OUPUT);
pinMode(Amarillo, OUTPUT);
pinMode(verde, OUTPUT);

void loop()[ 
digitalWrite(rojo, HIGH);
delay(5000);
digitalWrite(rojo, LOW);

digitaWrite(amarillo, HIGHT);
delay(4000);
digitalWrite(amarillo, LOW);

digitalWrite(verde; HIGHT);
delay(2000);
digitalWrite(verde;LOW);
]
```
Lanzamos y esperamos que Arduino ejecute el proceso, puedes variar los tiempos del delay según los segundos que quieres que demore en cada transición.

<img width="2296" height="4080" alt="20260930_194307" src="https://github.com/user-attachments/assets/cc54a3cf-b97e-489c-b316-c3b82a95d4da" />
