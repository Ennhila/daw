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

# Unidad 2

***

{% hint style="danger" %}
Si alguna de las soluciones de los ejercicios es incorrecta, no dudes en contactarme.
{% endhint %}

### Actividad 1 P26

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

{% code fullWidth="false" %}
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
{% endcode %}

### Actividad 5 P34

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>
#include <math.h>

int main() {
    float lado1, lado2, diagonal;
    
    // Pedir al usuario que introduzca las longitudes de los lados del rectángulo
    printf("Introduce la longitud del primer lado del rectángulo: ");
    scanf("%f", &lado1);
    printf("Introduce la longitud del segundo lado del rectángulo: ");
    scanf("%f", &lado2);
    
    // Calcular la longitud de la diagonal usando el teorema de Pitágoras
    diagonal = sqrt(pow(lado1, 2) + pow(lado2, 2));
    
    // Mostrar el resultado
    printf("La longitud de la diagonal del rectángulo es: %.2f\n", diagonal);
    
    return 0;
}

```

### Actividad 6 P35

<figure><img src="../../.gitbook/assets/image (5) (1) (1).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>
#include <stdlib.h>
#include <math.h>

int main(){
	
	int Ax, Ay, Bx, By;
	
	printf("dame el punto Ax de el vector A: \n");
	scanf("%d", &Ax);
	printf("dame el punto Ay de el vector A: \n");
	scanf("%d", &Ay);
	
	printf("dame el punto Bx de el vector B: \n");
	scanf("%d", &Bx);
	printf("dame el punto By de el vector B: \n");
	scanf("%d", &By);
	
	//Calcula el Vector AB
	float ABx = Bx-Ax;
	float ABy = By-Ay;
	
	//Calcula el modulo de AB
	float modulo = sqrt ( (ABx) * (ABx) + (ABy) * (ABy));
	
	//Calcula el vector unitario
	float unitarioX = (ABx) / modulo;
	float unitarioY = (ABy) / modulo;
	
	
	printf("El Vector AB (%.1f,%.1f)\n", ABx, ABy );
	printf("El modulo de AB es: %.1f\n", modulo);
	printf("\n El verctor unitario: u(%.1f,%.1f)", unitarioX, unitarioY);

}
```

### Actividad 7 P37

<figure><img src="../../.gitbook/assets/image (6) (1).png" alt=""><figcaption></figcaption></figure>

```c
//Actividad 7: Area del circulo
#include <stdio.h>

// Definimos la variable global para el valor de PI
#define PI 3.1415

int main() {
    float radio, area;

    printf("Introduce el radio del circulo: ");
    scanf("%f", &radio);

    // Calculamos el área del círculo
    area = PI * radio * radio;

    // Mostramos el resultado
    printf("El area del circulo es: %.2f\n", area);

    return 0;
}
```

### Actividad 8 P37

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

```c
//Actividad 8: Menu
#include <stdio.h>

int main() {
    int opcion;

    // Mostrar el menu de opciones
    printf("Menu de opciones:\n");
    printf("1. Opcion 1\n");
    printf("2. Opcion 2\n");
    printf("3. Opcion 3\n");
    printf("4. Salir\n");

    printf("Elija una opcion (1-4): ");
    scanf("%d", &opcion);

	printf("\nLa opcion elegida es: %d", opcion);
	
	return 0;
}
```

### Actividad 9 P37

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

```c
//ACTIVIDAD 9 - Precio medio


#include <stdio.h>

int main(){
	
	float precio1, precio2, precio3, precio4, precioMedio;
	
	printf("\nIntroduce el precio del producto en establecimiento 1: ");
	scanf("%f", &precio1);
	
	printf("\nIntroduce el precio del producto en establecimiento 2: ");
	scanf("%f", &precio2);
	
	printf("\nIntroduce el precio del producto en establecimiento 3: ");
	scanf("%f", &precio3);
	
	printf("\nIntroduce el precio del producto de establecimiento 4: ");
	scanf("%f", &precio4);
	
	precioMedio = ( precio1 + precio2 + precio3 + precio4 ) / 4;
	
	printf("\nEl precio medio del productos es: %.2f", precioMedio);
	
	return 0;
}
```

### Actividad 10 P38

<figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>
#include <math.h>
#define PI 3.1415
int main (){
	
	float grados, radianes;
	
	printf("Introduce los grados: ");
	scanf("%f", &grados);
	
	//operacion -> 180 - pi
	//				gra - x
	radianes = (grados * PI) / 180;
	
	printf("%f grados son %f radianes", grados, radianes);
	
	
}
```

### Actividad 11 P38

```c
//Actividad 11 - Operaciones matematicas
#include <stdio.h>
#include <math.h>


int main() {
	
	float num;
	
	printf("Introduce un numero real mayor que cero: ");
	scanf("%f", &num);
	
	printf("El numero introducido es: %.2f", num);
	printf("\nCuadrado: %.2f", num * num);
	printf("\nCubo: %.2f", num * num * num);
	printf("\nLogaritmo neperiano: %.3f", log(num) );
	printf("\nRaiz cuadrada: %.3f", sqrt(num));
	
}
```

### Actividad 12 P39

<figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main() {
    int horas1, minutos1, segundos1;
    int horas2, minutos2, segundos2;
    int total_segundos1, total_segundos2;
    
    // Pedir al usuario que introduzca el tiempo de estudio del primer alumno
    printf("Introduce las horas, minutos y segundos que ha estudiado el primer alumno:\n");
    printf("Horas: ");
    scanf("%d", &horas1);
    printf("Minutos: ");
    scanf("%d", &minutos1);
    printf("Segundos: ");
    scanf("%d", &segundos1);
    
    // Convertir el tiempo total del primer alumno a segundos
    total_segundos1 = horas1 * 3600 + minutos1 * 60 + segundos1;
    
    // Pedir al usuario que introduzca el tiempo de estudio del segundo alumno
    printf("Introduce las horas, minutos y segundos que ha estudiado el segundo alumno:\n");
    printf("Horas: ");
    scanf("%d", &horas2);
    printf("Minutos: ");
    scanf("%d", &minutos2);
    printf("Segundos: ");
    scanf("%d", &segundos2);
    
    // Convertir el tiempo total del segundo alumno a segundos
    total_segundos2 = horas2 * 3600 + minutos2 * 60 + segundos2;
    
    // Mostrar los resultados
    printf("Alumno 1: %d horas, %d minutos y %d segundos son un total de %d segundos.\n", horas1, minutos1, segundos1, total_segundos1);
    printf("Alumno 2: %d horas, %d minutos y %d segundos son un total de %d segundos.\n", horas2, minutos2, segundos2, total_segundos2);
    
    // Comparar los tiempos de estudio
    if (total_segundos1 > total_segundos2) {
        printf("El primer alumno ha estudiado más.\n");
    } else if (total_segundos1 < total_segundos2) {
        printf("El segundo alumno ha estudiado más.\n");
    } else {
        printf("Ambos alumnos han estudiado el mismo tiempo.\n");
    }
    
    return 0;
}
```

### Actividad 13 P39

<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

```c
//Actividad 13 - Cambios Unidad II

#include <stdio.h>
#include <math.h>

int main() {
    int segundos, horas, minutos, segundos_restantes;
    printf("Introduce la cantidad de segundos: ");
    scanf("%d", &segundos);

    
    horas = segundos / (60 * 60);
    segundos_restantes = segundos % (60 * 60);
    minutos = segundos_restantes / 60;
    segundos_restantes = segundos_restantes % 60;

    
    printf("%d segundos son %d horas, %d minutos y %d segundos.\n", segundos, horas, minutos, segundos_restantes);

    return 0;
}
```

