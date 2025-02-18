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