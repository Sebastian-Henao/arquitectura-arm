
***Introducción a la Arquitectura ARM***

La arquitectura ARM (Advanced RISC Machine) es una de las arquitecturas de procesadores más utilizadas en 
el mundo, especialmente en dispositivos móviles, sistemas embebidos y servidores de bajo consumo. Se basa en un conjunto de instrucciones de tipo RISC (Reduced Instruction Set Computing), lo que la hace eficiente en términos de consumo energético y rendimiento.

**Historia y Evolución**

ARM tiene sus orígenes en la década de 1980 con Acorn Computers, que diseñó el primer procesador basado en esta arquitectura para computadoras personales; con el tiempo, la empresa ARM Holdings (ahora propiedad de NVIDIA, tras ser adquirida de SoftBank) desarrolló y licenciaba estos procesadores a diversas compañías.

*Características Principales*
- Arquitectura RISC: Usa un conjunto reducido de instrucciones, optimizando velocidad y eficiencia energética.
- Licenciamiento: ARM no fabrica chips, sino que licencia su tecnología a fabricantes como Apple, Qualcomm y Samsung.
- Bajo consumo energético: Ideal para dispositivos móviles, IoT y sistemas embebidos.
- Extensibilidad: Permite personalización por parte de los fabricantes.
Modos de ejecución: Soporta diferentes niveles de ejecución, como modo usuario y supervisor.

*Usos Comunes*

- Teléfonos y tablets (Apple, Samsung, Qualcomm Snapdragon).
- Dispositivos IoT y embebidos (Raspberry Pi, microcontroladores).
- Servidores y computación en la nube (AWS Graviton, Ampere Altra).
- Automóviles y sistemas industriales.

**Futuro de ARM**

Con la creciente adopción de ARM en servidores y la evolución hacia ARMv9, esta arquitectura sigue expandiéndose y ganando terreno frente a x86 en diversas aplicaciones.


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

### ***INSTRUCCIONES DE ARM***

ARM utiliza un conjunto reducido de instrucciones, lo que simplifica la ejecución y mejora el rendimiento. Existen distintos tipos de instrucciones en ARM, entre ellas:

**Instrucciones de transferencia de datos:**

 - **MOV:** Mueve un valor a un registro.

 - **LDR:** Carga un valor desde memoria a un registro.

 - **STR:** Almacena el valor de un registro en memoria.

**Instrucciones aritméticas y lógicas:**

 - **ADD:** Suma valores y almacena el resultado en un registro.

 - **SUB:** Resta valores y almacena el resultado en un registro.

 - **MUL:** Multiplica dos registros y almacena el resultado.

 - **AND, ORR, EOR:** Operaciones lógicas AND, OR y XOR

**Instrucciones de comparación y control de flujo:**

 - **CMP:** Compara dos valores.

 - **B:** Salto incondicional a una dirección específica.

 - **BL:** Llamada a subrutina.

 - **BX:** Retorno de subrutina o cambio de estado del procesador.

Además, ARM posee características avanzadas como:

**Ejecución condicional:** Todas las instrucciones pueden ejecutarse condicionalmente en función del estado de las banderas del registro CPSR, lo que minimiza la necesidad de saltos y mejora la eficiencia.

**Formato de tres operandos:** Permite especificar dos operandos fuente y un operando destino en una sola instrucción, reduciendo la cantidad de instrucciones requeridas.

**Manipulación eficiente de bits:** ARM permite realizar operaciones de desplazamiento y rotación de bits en la misma instrucción, optimizando el procesamiento de datos.

**Carga y almacenamiento múltiples:** Instrucciones como LDM y STM permiten manipular varios registros simultáneamente, acelerando el acceso a la memoria.

**Extensibilidad mediante coprocesadores:** ARM permite la integración de coprocesadores especializados, lo que expande las capacidades del procesador sin afectar su rendimiento general.

Estas características hacen que la arquitectura ARM sea altamente eficiente y adecuada para una amplia gama de aplicaciones, desde dispositivos móviles hasta sistemas embebidos y servidores de alto rendimiento.

