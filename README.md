# assembler-pic-desplazamiento-led
El programa simula un efecto de "desplazamiento" en los LEDs

Resumen breve:
Configuración Inicial:

Usa el oscilador interno.
Configura TRISA y TRISB como salidas para los puertos A y B.
Desactiva los comparadores analógicos (usando CMCON).
Macro CONTROL_LED:

Permite escribir un valor en un registro específico, en este caso en PORTB para controlar los LEDs.
Bucle Principal (MAIN_LOOP):

Enciende secuencialmente los pines del Puerto B desde 0x01 (primer LED) hasta 0x80 (último LED), creando un efecto de "carrera de luces".
Llama a la subrutina retardo entre cada encendido para ralentizar el patrón.
Subrutina de Retardo (retardo):

Implementa un retardo mediante la disminución de varios registros (cout_1 a cout_4) en bucles anidados para hacer visible el encendido secuencial de los LEDs.
