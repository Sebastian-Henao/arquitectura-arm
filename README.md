# Registros en ARM

Un procesador ARM tiene varios tipos de registros, que pueden variar según la versión de la arquitectura. 

## Registros de propósito general (GPR - General Purpose Registers)

- **En ARM de 32 bits, hay 16 registros de propósito general:**

  - R0-R12: Uso general.
  - R13 (SP - Stack Pointer): Puntero de pila.
  - R14 (LR - Link Register): Almacena la dirección de retorno de una subrutina.
  - R15 (PC - Program Counter): Contiene la dirección de la siguiente instrucción a ejecutar.

- **En ARM de 64 bits, hay 31 registros de propósito general (X0-X30):**

  - X0-X28: Uso general.b
  - X29 (FP - Frame Pointer): Para almacenamiento de marcos de pila.
  - X30 (LR - Link Register): Para almacenar la dirección de retorno de llamadas a funciones.


