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

***

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
    int i;

	for(i =1; i<=100;i++){
		printf("%d ", i);
		if(i%10==0){
			printf("\n");
		}
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

### Actividad 12 P29

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main(){
	int num, a, i;
	
	printf("dame num:	");
	scanf("%d", &num);
	printf("\n");
	a=1;
	while(a<=num){
		i=0;
		while(i<=10){
			printf("%d*%d=%d\n", a, i, a*i);
			i++;
		}
		a=a+1;
	}
}
```

### Actividad 13 P29

<figure><img src="../../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    int n;
    float suma = 0.0;


    do {
        printf("Introduce un valor para n (1 <= n <= 30000): ");
        scanf("%d", &n);
        if (n < 1 || n > 30000) {
            printf("Valor no valido. Por favor, intentalo de nuevo.\n");
        }
    } while (n < 1 || n > 30000);


    for (int i = 1; i <= n; i++) {
        suma += (float)i / (i + 1);
    }


    printf("La suma de la serie es: %.6f\n", suma);

    return 0;
}
```

### Actividad 14 P29

<figure><img src="../../.gitbook/assets/image (2) (1) (1).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main(){
	int n, suma;
	printf("Introduce un num: ");
	scanf("%d", &n);
	
	for(int i = 1; i<=n; i++){
		suma += pow(i, 2);
	}
	printf("la suma de la serie es: %d\n", suma);
}
```

### Actividad 15 P30

<figure><img src="../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main (){
	int num, res=0;
	while (1){
		printf("Num: ");
		scanf("%d", &num);
		if(num<=0){
			break;
		}
		
		res = res + num;
	}
	printf("\nSuma: %d\n", res);
}
```

### Actividad 16 P30

<figure><img src="../../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main(){
	int i, num, fact=1;
	printf("Introduce num: ");
	scanf("%d", &num);
	
	for(i=1; i <= num; i++){
		fact = fact*i;
		printf("%d! = %d\n", i, fact);
	}
	
}
```

### Actividad 17 P30

<figure><img src="../../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main(){
	int i, num;
	int suma=0;
	do{
		printf("Introduce num:");
		scanf("%d", &num);
		suma = suma + num;
		i++;
	}while(num!=0);
	float media = (float)suma/(i - 1);
	printf("Media: %.2f", media);
	
}
```

### Actividad 18 P30

<figure><img src="../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    int n1 = 0, n2 = 1, nextTerm, i;

    printf("Los primeros 30 números de la sucesión de Fibonacci son:\n");
    printf("%d, %d", n1, n2);

    for (i = 3; i <= 30; i++) {
        nextTerm = n1 + n2;
        printf(", %d", nextTerm);
        n1 = n2;
        n2 = nextTerm;
    }

    printf("\n");

    return 0;
}
```

### Actividad 19 P31

<figure><img src="../../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    int altura;
    char caracter;

    
    printf("Introduce un número entero: ");
    scanf("%d", &altura);
    printf("Introduce un carácter: ");
    scanf(" %c", &caracter); 

    // Imprimir el carácter en forma de triángulo
    for (int i = 1; i <= altura; ++i) {
        for (int j = 1; j <= i; ++j) {
            printf("%c", caracter);
        }
        printf("\n");
    }

    return 0;
}
```

### Actividad 20 P31

<figure><img src="../../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    int altura;
    char caracter;

    
    printf("Introduce un número entero: ");
    scanf("%d", &altura);
    printf("Introduce un carácter: ");
    scanf(" %c", &caracter); 

    // Parte superior del rombo (ascendente)
    for (int i = 1; i <= altura; ++i) {
        for (int j = 1; j <= i; ++j) {
            printf("%c", caracter);
        }
        printf("\n");
    }

    // Parte inferior del rombo (descendente)
    for (int i = altura - 1; i >= 1; --i) {
        for (int j = 1; j <= i; ++j) {
            printf("%c", caracter);
        }
        printf("\n");
    }

    return 0;
}

```

### Actividad 21 P31

<figure><img src="../../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>
#include <math.h>

int main() {
    float a, b, c;
    float discriminante, raiz1, raiz2, parteReal, parteImaginaria;

    // Solicitar los coeficientes a, b y c
    printf("Introduce el valor de a: ");
    scanf("%f", &a);
    printf("Introduce el valor de b: ");
    scanf("%f", &b);
    printf("Introduce el valor de c: ");
    scanf("%f", &c);

    // Calcular el discriminante
    discriminante = b * b - 4 * a * c;

    // Verificar si el discriminante es mayor, igual o menor que 0
    if (discriminante > 0) {
        // Dos raíces reales y diferentes
        raiz1 = (-b + sqrt(discriminante)) / (2 * a);
        raiz2 = (-b - sqrt(discriminante)) / (2 * a);
        printf("Las raíces son reales y diferentes: %.2f y %.2f\n", raiz1, raiz2);
    } 
    else if (discriminante == 0) {
        // Una raíz real (raíz doble)
        raiz1 = -b / (2 * a);
        printf("La raíz es real y doble: %.2f\n", raiz1);
    } 
    else {
        // Raíces complejas
        parteReal = -b / (2 * a);
        parteImaginaria = sqrt(-discriminante) / (2 * a);
        printf("Las raíces son complejas: %.2f + %.2fi y %.2f - %.2fi\n", parteReal, parteImaginaria, parteReal, parteImaginaria);
    }

    return 0;
}

```

### Actividad 22 P31

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    int numero;
    do {
        printf("Introduce un número (introduce un número negativo para salir): ");
        scanf("%d", &numero);

        if (numero >= 0) {
            printf("Has introducido: %d\n", numero);
        }
    } while (numero >= 0);

    printf("Número negativo introducido. Fin del programa.\n");

    return 0;
}

```

### Actividad 23 P32

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    int nota, totalAlumnos = 0, sobresalientes = 0, notables = 0, aprobados = 0, suspensos = 0;
    float sumaNotas = 0.0;

    printf("Introduzca las notas (número negativo para terminar):\n");
    while (1) {
        scanf("%d", &nota);
        if (nota < 0) break;
        sumaNotas += nota;
        totalAlumnos++;
        if (nota >= 9) sobresalientes++;
        else if (nota >= 7) notables++;
        else if (nota >= 5) aprobados++;
        else suspensos++;
    }

    if (totalAlumnos > 0) {
        float notaMedia = sumaNotas / totalAlumnos;
        printf("Total alumnos: %d\n", totalAlumnos);
        printf("Total sobresalientes: %d\n", sobresalientes);
        printf("Total notables: %d\n", notables);
        printf("Total aprobados: %d\n", aprobados);
        printf("Total suspensos: %d\n", suspensos);
        printf("Nota media: %.2f\n", notaMedia);
        printf("Porcentaje sobresalientes: %.2f%%\n", (sobresalientes * 100.0) / totalAlumnos);
        printf("Porcentaje notables: %.2f%%\n", (notables * 100.0) / totalAlumnos);
        printf("Porcentaje aprobados: %.2f%%\n", (aprobados * 100.0) / totalAlumnos);
        printf("Porcentaje suspensos: %.2f%%\n", (suspensos * 100.0) / totalAlumnos);
    } else {
        printf("No se han introducido notas.\n");
    }

    return 0;
}
```

