# 3.2 Registros en ARM

Un procesador ARM tiene varios tipos de registros, que pueden variar según la versión de la arquitectura. 

## Registros de propósito general (GPR - General Purpose Registers)

- **En ARM de 32 bits, hay 16 registros de propósito general:**

  - **R0-R12:** Uso general.
  - **R13 (SP - Stack Pointer):** Puntero de pila.
  - **R14 (LR - Link Register):** Almacena la dirección de retorno de una subrutina.
  - **R15 (PC - Program Counter):** Contiene la dirección de la siguiente instrucción a ejecutar.

- **En ARM de 64 bits, hay 31 registros de propósito general (X0-X30):**

  - **X0-X28:** Uso general.b
  - **X29 (FP - Frame Pointer):** Para almacenamiento de marcos de pila.
  - **X30 (LR - Link Register):** Para almacenar la dirección de retorno de llamadas a funciones.

## Registros de estado en ARM

- **CPSR (Current Program Status Register):** Indica el estado del procesador con bits de condición (N, Z, C, V) y bits de control.
- **SPSR (Saved Program Status Register):** Guarda el CPSR cuando se entra a una interrupción o cambio de modo.


# 5 La arquitectura ARM se utiliza en una variedad de aplicaciones y dispositivos debido a su eficiencia energética y rendimiento. algunos ejemplos son:

1) Smartphones y Tablets: La mayoría de los dispositivos móviles modernos, como los teléfonos inteligentes y tabletas, utilizan procesadores ARM debido a su bajo consumo de energía y duración de la batería prolongada.

2) Ordenadores Portátiles y Convertibles: Algunos ordenadores portátiles y convertibles, especialmente aquellos que buscan una mayor duración de la batería, utilizan procesadores ARM.

3) Sistemas Embebidos: Los sistemas embebidos, como los que se encuentran en electrodomésticos inteligentes, automóviles y dispositivos IoT (Internet de las Cosas), a menudo utilizan procesadores ARM.

4) Servidores y Centros de Datos: Algunos servidores y centros de datos están comenzando a adoptar procesadores ARM debido a su eficiencia energética y capacidad de manejar cargas de trabajo específicas.

5) Dispositivos de Realidad Aumentada y Virtual: Algunos dispositivos de realidad aumentada y virtual también utilizan procesadores ARM para su eficiencia y rendimiento