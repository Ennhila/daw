# Unidad 2

### Actividad 1 P26

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    int numero;
    
    // Pedir al usuario que introduzca un número entero
    printf("Introduce un número entero: ");
    scanf("%d", &numero);
    
    // Calcular el doble del número
    int doble = numero * 2;
    
    // Mostrar el resultado
    printf("El doble de %d es %d\n", numero, doble);
    
    return 0;
}

```

### Actividad 3 P27

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    float celsius, fahrenheit;
    
    // Pedir al usuario que introduzca los grados centígrados
    printf("Introduce la cantidad de grados centígrados: ");
    scanf("%f", &celsius);
    
    // Convertir a grados Fahrenheit
    fahrenheit = (celsius * 9 / 5) + 32;
    
    // Mostrar el resultado
    printf("%.2f grados centígrados son %.2f grados Fahrenheit\n", celsius, fahrenheit);
    
    return 0;
}

```
