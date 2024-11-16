# assembler-pic-desplazamiento-led
El programa simula un efecto de "desplazamiento" en los LEDs


Configuración Inicial: Configura el Puerto A como entradas y el Puerto B como salidas. Desactiva los comparadores internos para liberar los pines.
Bucle Principal: Lee un valor del Puerto A y ejecuta un patrón específico en el Puerto B dependiendo de dicho valor. Si el valor corresponde a 0-9, muestra un patrón girando hacia la derecha (turn_right). Si no, gira hacia la izquierda (turn_left).
Subrutinas de Movimiento:
turn_right: Enciende secuencialmente LEDs conectados al puerto B en una dirección.
turn_left: Enciende los LEDs en la dirección opuesta.
Retardo (Deley): Implementa un pequeño retardo para hacer visibles los patrones de luces.
