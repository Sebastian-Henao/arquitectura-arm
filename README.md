# 4 Codigo De Ejemplo

'.global _start

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
    swi 0                // Interrupción del sistema para hacer la llamada'

## Explicación

1. **_start:** Es la etiqueta donde empieza el programa.
2. **mov r0, #5:** Carga el valor 5 en el registro r0.
3. **mov r1, #10:** Carga el valor 10 en el registro r1.
4. **add r0, r0, r1:** Realiza la suma de los valores en los registros r0 y r1, y almacena el resultado en r0.
5. **mov r7, #1:** Prepara la llamada al sistema para terminar el programa.
6. **swi 0:** Genera una interrupción para finalizar la ejecución.