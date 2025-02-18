# 1 Introducción a la Arquitectura ARM

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

# 2 Historia

Orígenes (1980 - 1990)  
La historia de ARM comenzó en **Acorn Computers**, una empresa británica que desarrollaba computadoras personales. En 1983, Acorn necesitaba un procesador más eficiente para sus computadoras y decidió diseñar su propia arquitectura basada en la filosofía **RISC (Reduced Instruction Set Computing)**, que simplifica las instrucciones del procesador para mejorar el rendimiento y reducir el consumo de energía.  

En 1985, Acorn lanzó el **Acorn RISC Machine (ARM1)**, su primer procesador RISC de 32 bits. Poco después, en 1987, apareció el **ARM2**, que fue utilizado en la computadora **Acorn Archimedes**. Este procesador destacaba por su eficiencia energética y buen rendimiento en comparación con otros de la época.  

### **Fundación de ARM Ltd. (1990 - 2000)**  
En 1990, **Acorn Computers**, junto con **Apple** y **VLSI Technology**, fundaron la empresa **Advanced RISC Machines Ltd.** (ARM Ltd.), con el objetivo de diseñar y licenciar procesadores basados en su arquitectura.  

Durante los años 90, ARM creció rápidamente debido a su modelo de negocio de **licencias**, donde otras empresas podían diseñar sus propios chips basados en la arquitectura ARM sin necesidad de fabricar los procesadores directamente. Esto permitió su adopción en una gran variedad de dispositivos embebidos.  

En 1993, ARM lanzó el **ARM6**, y en 1994, el **ARM7**, que fue ampliamente utilizado en dispositivos portátiles y embebidos.  

### **Expansión con dispositivos móviles (2000 - 2010)**  
En los 2000, ARM se convirtió en el estándar para dispositivos móviles. La mayoría de los primeros teléfonos celulares y asistentes digitales personales (PDA) usaban procesadores ARM debido a su **bajo consumo energético**.  

En 2003, se introdujo la familia **ARM Cortex**, con procesadores como el **Cortex-A**, destinado a aplicaciones de alto rendimiento, y el **Cortex-M**, diseñado para sistemas embebidos y microcontroladores.  

El gran salto llegó con la revolución de los teléfonos inteligentes. En 2007, el **iPhone de Apple** usó un procesador basado en ARM, marcando una nueva era para la computación móvil. Android, lanzado en 2008, también adoptó ARM como su arquitectura principal.  

### **Dominio del mercado y nuevas innovaciones (2010 - 2020)**  
Durante la década de 2010, ARM consolidó su dominio en los dispositivos móviles. La mayoría de los **smartphones, tablets y dispositivos IoT** funcionaban con procesadores basados en ARM.  

En 2016, la empresa **SoftBank** adquirió ARM Ltd. por **32 mil millones de dólares**, con el objetivo de expandir su presencia en inteligencia artificial y computación en la nube.  

En 2020, **Apple anunció la transición de sus Mac** a procesadores basados en ARM con la serie **Apple M1**, lo que demostró que ARM podía competir con procesadores de alto rendimiento como los de Intel y AMD.  

### **Actualidad y futuro (2020 - presente)**  
Hoy en día, ARM es una de las arquitecturas más utilizadas en el mundo. No solo domina los teléfonos inteligentes, sino que también se ha expandido a servidores, automóviles, computadoras portátiles y dispositivos de alto rendimiento. Empresas como **Qualcomm, NVIDIA, Samsung y Apple** siguen desarrollando procesadores avanzados basados en ARM.  

# Introducción al Lenguaje Ensamblador

## Descripción
El lenguaje ensamblador es un lenguaje de bajo nivel que se utiliza para programar directamente el hardware de una computadora. Se compone de instrucciones mnemotécnicas que representan operaciones específicas que la CPU puede ejecutar.

## Características del Lenguaje Ensamblador
- Comunicación directa con el hardware.
- Alto rendimiento y eficiencia en el uso de recursos.
- Dependiente de la arquitectura del procesador.
- Utiliza registros y memoria de manera explícita.

## Uso del Lenguaje Ensamblador
El ensamblador se usa en:
- Programación de sistemas embebidos.
- Desarrollo de controladores de dispositivos.
- Optimización de código crítico en software de alto rendimiento.
- Análisis de malware y seguridad informática.

## Instrucciones Básicas
Algunas de las instrucciones comunes en ensamblador incluyen:
- `MOV`: Mueve datos de un lugar a otro.
- `ADD`: Suma valores.
- `SUB`: Resta valores.
- `JMP`: Salta a una dirección específica de código.
- `CMP`: Compara valores.

## Ensambladores Populares
Existen varios ensambladores que permiten programar en este lenguaje, como:
- NASM (Netwide Assembler)
- MASM (Microsoft Macro Assembler)
- GAS (GNU Assembler)
- FASM (Flat Assembler)

## Conclusión
El lenguaje ensamblador es una herramienta poderosa para la programación de bajo nivel. Aunque su uso ha disminuido con lenguajes de alto nivel, sigue siendo esencial en aplicaciones donde el control del hardware es crítico.

# 3.1 Instrucciones

***INSTRUCCIONES DE ARM***

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

#

# 4 Codigo De Ejemplo

Este código sirve para realizar una suma de dos números y mostrar el resultado.

    .global _start

    .section .text
    _start:
        // Cargar el primer número en el registro r0
        mov r0, #5           // r0 = 5

        // Cargar el segundo número en el registro r1
        mov r1, #10          // r1 = 10

        // Sumar los valores en r0 y r1 y almacenar el resultado en r0
        add r0, r0, r1       // r0 = r0 + r1 => 5 + 10 = 15

        // Aquí podrías agregar un código para mostrar el resultado en pantalla
        // Sin embargo, este es un ejemplo simple, por lo que solo terminará la ejecución

        // Salir del programa
        mov r7, #1           // syscall para terminar el programa
        swi 0                // Interrupción del sistema para hacer la llamada

## Explicación

1. **_start:** Es la etiqueta donde empieza el programa.
2. **mov r0, #5:** Carga el valor 5 en el registro r0.
3. **mov r1, #10:** Carga el valor 10 en el registro r1.
4. **add r0, r0, r1:** Realiza la suma de los valores en los registros r0 y r1, y almacena el resultado en r0.
5. **mov r7, #1:** Prepara la llamada al sistema para terminar el programa.
6. **swi 0:** Genera una interrupción para finalizar la ejecución.

# 5 Aplicaciones

La arquitectura ARM se utiliza en una variedad de aplicaciones y dispositivos debido a su eficiencia energética y rendimiento. algunos ejemplos son:

1) Smartphones y Tablets: La mayoría de los dispositivos móviles modernos, como los teléfonos inteligentes y tabletas, utilizan procesadores ARM debido a su bajo consumo de energía y duración de la batería prolongada.

2) Ordenadores Portátiles y Convertibles: Algunos ordenadores portátiles y convertibles, especialmente aquellos que buscan una mayor duración de la batería, utilizan procesadores ARM.

3) Sistemas Embebidos: Los sistemas embebidos, como los que se encuentran en electrodomésticos inteligentes, automóviles y dispositivos IoT (Internet de las Cosas), a menudo utilizan procesadores ARM.

4) Servidores y Centros de Datos: Algunos servidores y centros de datos están comenzando a adoptar procesadores ARM debido a su eficiencia energética y capacidad de manejar cargas de trabajo específicas

5) Dispositivos de Realidad Aumentada y Virtual: Algunos dispositivos de realidad aumentada y virtual también utilizan procesadores ARM para su eficiencia y rendimient

Otras de sus aplicaciones son en la creacion de microprocesadores, desde los mas simples, hasta para ordenadores personales, algunas
de los dispositivos que usan estos microprocesadores son las IPad Pro de Apple.

# Anexo

El flujo del trabajo del TEAM 5 se realizo, creando el repositorio con la rama main como principal, luego se genera la rama development
en la cual se genera un archivo README.md vacio, cada miembro del grupo genera una rama nueva desde la ya existente development, cada uno 
llena su archivo con la informacion del tema asignado, subiendolo a su rama, por ultimo, usando los comandos "git switch (o git checkout) development",
"git pull", "git merge" con el nombre de su rama, en caso de generar conflictos, se deben solucionar borrando todo lo innecesario y organizando el contenido,
por ultimo se realiza un "git add .", "git commit -m "descripcion del cambio" y un "git push origin development", logrando asi fusionar el trabajo
realizado en cada rama en la rama development
