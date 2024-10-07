---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Unidad 3

{% hint style="danger" %}
Si alguna de las soluciones de los ejercicios es incorrecta, no dudes en contactarme.
{% endhint %}

### Actividad 1 P17

<figure><img src="../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>
#include <math.h>

int main() {
    int opcion;
    float base, altura, radio, area;

    do {
        // Mostrar el menú de opciones
        printf("\nSeleccione una opción:\n");
        printf("a) Área de un rectángulo\n");
        printf("b) Área de un triángulo\n");
        printf("c) Área de un círculo\n");
        printf("d) Salir\n");
        printf("Opción: ");
        opcion = getchar();
        getchar(); // Para capturar el salto de línea

        switch(opcion) {
            case 'a':
                // Pedir base y altura para el rectángulo
                printf("Introduce la base del rectángulo: ");
                scanf("%f", &base);
                printf("Introduce la altura del rectángulo: ");
                scanf("%f", &altura);
                area = base * altura;
                printf("El área del rectángulo es: %.2f\n", area);
                break;
            case 'b':
                // Pedir base y altura para el triángulo
                printf("Introduce la base del triángulo: ");
                scanf("%f", &base);
                printf("Introduce la altura del triángulo: ");
                scanf("%f", &altura);
                area = (base * altura) / 2;
                printf("El área del triángulo es: %.2f\n", area);
                break;
            case 'c':
                // Pedir radio para el círculo
                printf("Introduce el radio del círculo: ");
                scanf("%f", &radio);
                area = M_PI * radio * radio;
                printf("El área del círculo es: %.2f\n", area);
                break;
            case 'd':
                printf("Saliendo del programa...\n");
                break;
            default:
                printf("Opción no válida. Por favor, seleccione una opción válida.\n");
        }

        // Limpiar el buffer de entrada
        while (getchar() != '\n');

    } while(opcion != 'd');

    return 0;
}

```

### Actividad 2 P18

<figure><img src="../../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>
#include <math.h>

int main() {
    double x, resultado;

    // Pedir al usuario que introduzca el valor de x
    printf("Introduce el valor de x: ");
    scanf("%lf", &x);

    // Calcular el valor de f(x) según la definición de la función por partes
    if (x >= 2 && x <= 5) {
        resultado = log(x);
    } else if (x >= -1 && x <= 2) {
        resultado = exp(x - 1);
    } else if (x > 5) {
        resultado = pow(x, 2) - 2 * x;
    } else if (x < -1) {
        resultado = pow(x, 3) - x;
    } else {
        printf("Valor de x fuera del rango definido.\n");
        return 1;
    }

    // Mostrar el resultado
    printf("El valor de f(%.2f) es %.2f\n", x, resultado);

    return 0;
}

```

### Actividad 3 P19

<figure><img src="../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

```c
//Actividad 3 UD3

#include <stdio.h>


int main (){
	int num, dec, uds;
	printf("Introduce un numero [10-99]:	");
	scanf("%d", &num);
	
	if (num>=10 && num<=99){
		dec = num / 10;
		uds = num % 10;
		printf("Decenas: %d\nUnidades: %d\n\n", dec, uds);
		
		switch(dec){
			case 0:
				printf("C");
				break;
			case 1:
				printf("E");
				break;
			case 2:
				printf("N");
				break;
			case 3:
				printf("T");
				break;
			case 4:
				printf("R");
				break;
			case 5:
				printf("I");
				break;
			case 6:
				printf("F");
				break;
			case 7:
				printf("U");
				break;
			case 8:
				printf("G");
				break;
			case 9:
				printf("A");
				break;
			default:
				printf("NADA");
		}
		switch(uds){
			case 0:
				printf("C");
				break;
			case 1:
				printf("E");
				break;
			case 2:
				printf("N");
				break;
			case 3:
				printf("T");
				break;
			case 4:
				printf("R");
				break;
			case 5:
				printf("I");
				break;
			case 6:
				printf("F");
				break;
			case 7:
				printf("U");
				break;
			case 8:
				printf("G");
				break;
			case 9:
				printf("A");
				break;
			default:
				printf("NADA");
		}
	}else{
		printf("numero incorrecta");
	}
}
```

### Actividad 4 P26

<figure><img src="../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    int i;

	//while
    printf("Usando bucle while:\n");
    i = 0;
    while (i <= 10) {
        printf("%d ", i);
        i++;
    }
    printf("\n");
    i = 10;
    while (i >= 0) {
        printf("%d ", i);
        i--;
    }
    printf("\n\n");

	//do- while
    printf("Usando bucle do-while:\n");
    i = 0;
    do {
        printf("%d ", i);
        i++;
    } while (i <= 10);
    printf("\n");
    i = 10;
    do {
        printf("%d ", i);
        i--;
    } while (i >= 0);
    printf("\n\n");

	//For
    printf("Usando bucle for:\n");
    for (i = 0; i <= 10; i++) {
        printf("%d ", i);
    }
    printf("\n");
    for (i = 10; i >= 0; i--) {
        printf("%d ", i);
    }
    printf("\n");

    return 0;
}
```

### Actividad 5 P26

<figure><img src="../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

```c
int main (){

	int a, b;
	printf("Introduce el primero numero : \n");
	scanf("%d", &a);
	
	printf("Introduce el segundo numero : \n");
	scanf("%d", &b);
	
	printf("Tabla de multiplicar del %d:\n", a);
    for (int i = 0; i <= b; i++) {
        printf("%d x %d = %d\n", a, i, a * i);
    }
	printf("\n\n");
	
}
```

### Actividad 6 P26

<figure><img src="../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

```c
//Actividad 6 
#include <stdio.h>

int main(){

	printf("\nActividad 6 - Numeros impares");
	int num;
	printf("\nIntroduce un numero: ");
	scanf("%d", &num);
	
	for ( int i = 1; i <= num; i++){
		if(i % 2!=0){
			printf("%d", i);
		}
	}
}
```

### Actividad 7 P26

<figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    int n, suma = 0;

    // Pedir al usuario que introduzca el valor de n
    printf("Introduce el valor de n: ");
    scanf("%d", &n);

    // Calcular la suma de los primeros n números
    for (int i = 1; i <= n; i++) {
        suma += i;
    }

    // Mostrar el resultado
    printf("La suma de los primeros %d números es: %d\n", n, suma);

    return 0;
}
```

### Actividad 8 P28

<figure><img src="../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    int num, i, esPrimo = 1;

    
    printf("Introduce un numero: ");
    scanf("%d", &num);

    
    if (num < 2) {
        esPrimo = 0;
    } else {
        
        for (i = 2; i <= num / 2; i++) {
            if (num % i == 0) {
                esPrimo = 0;
                break;
            }
        }
    }


    if (esPrimo) {
        printf("%d es un numero primo.\n", num);
    } else {
        printf("%d no es un numero primo.\n", num);
    }

    return 0;
}
```

### Actividad 9 P28

<figure><img src="../../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    int numero, contador = 0;

    // Pedir al usuario que introduzca un número menor que 10
    printf("Introduce un número menor que 10: ");
    scanf("%d", &numero);

    // Verificar que el número es menor que 10
    if (numero >= 10) {
        printf("El número debe ser menor que 10.\n");
        return 1;
    }

    // Calcular el número de múltiplos entre 0 y 100
    for (int i = 1; i <= 100; i++) {
        if (i % numero == 0) {
            contador++;
        }
    }

    // Mostrar el resultado
    printf("Hay %d múltiplos de %d entre 0 y 100.\n", contador, numero);

    return 0;
}

```

### Actividad 10 P28

<figure><img src="../../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    int contador = 1;

    // Imprimir los números del 1 al 100 en una tabla de 10x10
    for (int fila = 0; fila < 10; fila++) {
        for (int columna = 0; columna < 10; columna++) {
            printf("%4d", contador);
            contador++;
        }
        printf("\n");
    }

    return 0;
}
```

### Actividad 11 P28

<figure><img src="../../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    char respuesta;

    do {
        printf("¿Desea salir? (S/N): ");
        scanf(" %c", &respuesta);
    } while (respuesta != 's' && respuesta != 'S');

    printf("Programa terminado.\n");
    return 0;
}

```

