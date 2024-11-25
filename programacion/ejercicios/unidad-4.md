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

# Unidad 4

***

### Actividad 1 P20

<figure><img src="../../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>
#define MAX_JUGADORES 6

int main(){
	int edad[MAX_JUGADORES];
	float puntuaciones[MAX_JUGADORES];
	float supervivencia[MAX_JUGADORES];
	char nombre[MAX_JUGADORES][20];
	
	for(int i = 0; i < MAX_JUGADORES; i++){
		printf("Introduce el nombre del jugador %d: ", i + 1);
		scanf("%s", nombre[i]);
		
		printf("Introduce la edad del jugador %d: ", i + 1);
		scanf("%d", &edad[i]);

        printf("Introduce la puntuacion del jugador %d: ", i + 1);
        scanf("%f", &puntuaciones[i]);

        printf("Introduce la tasa de supervivencia del jugador %d: ", i + 1);
        scanf("%f", &supervivencia[i]);
		
		printf("\n");
		getchar();
	}
	int sumaEdad = 0, sumaPuntuacion = 0;
    float sumaSupervivencia = 0.0;

    int minEdad = edad[0];
    int maxEdad = edad[0];
    float minPuntuacion = puntuaciones[0];
    float maxPuntuacion = puntuaciones[0];
    float minSupervivencia = supervivencia[0];
    float maxSupervivencia = supervivencia[0];

    for (int i = 0; i < MAX_JUGADORES; i++) {
        if (edad[i] < minEdad) minEdad = edad[i];
        if (edad[i] > maxEdad) maxEdad = edad[i];
        sumaEdad += edad[i];

        if (puntuaciones[i] < minPuntuacion) minPuntuacion = puntuaciones[i];
        if (puntuaciones[i] > maxPuntuacion) maxPuntuacion = puntuaciones[i];
        sumaPuntuacion += puntuaciones[i];

        if (supervivencia[i] < minSupervivencia) minSupervivencia = supervivencia[i];
        if (supervivencia[i] > maxSupervivencia) maxSupervivencia = supervivencia[i];
        sumaSupervivencia += supervivencia[i];
    }

    float promEdad = (float)sumaEdad / MAX_JUGADORES;
    float promPuntuacion = (float)sumaPuntuacion / MAX_JUGADORES;
	float promSupervivencia = sumaSupervivencia / MAX_JUGADORES;
	
	printf("\nEstadisticas generales:\n");
    printf("Edad - Minima: %d, Maxima: %d, Media: %.2f\n", minEdad, maxEdad, promEdad);
    printf("Puntuacion - Minima: %.2f, Maxima: %.2f, Media: %.2f\n", minPuntuacion, maxPuntuacion, promPuntuacion);
    printf("Tasa de supervivencia - Minima: %.2f, Máxima: %.2f, Media: %.2f\n", minSupervivencia, maxSupervivencia, promSupervivencia);
}
```

### Actividad 2 P21

<figure><img src="../../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>
#define DIAS 4
#define MDIAS 5

int main(){
	float temp[DIAS][MDIAS];
	int i, j;
	
	//ingresa la temperatura
	printf("Ingrese las temperaturas (4 dias, 5 muestras por dia):\n");
		for (int i = 0; i < DIAS; i++) {
        	for (int j = 0; j < MDIAS; j++) {
                printf("Dia %d, Muestra %d: ", i + 1, j + 1);
                scanf("%f", &temp[i][j]);
            }
            printf("\n");
		}
	  	
	float minTotal = temp[0][0];
    float maxTotal = temp[0][0];
 
        // Análisis de temperaturas
    for (int dia = 0; dia < 4; dia++) {
            float minDia = temp[dia][0];
            float maxDia = temp[dia][0];
            for (int i = 0; i < 5; i++) {
                if (temp[dia][i] < minDia) {
                    minDia = temp[dia][i];
                }
                if (temp[dia][i] > maxDia) {
                    maxDia = temp[dia][i];
                }
                // Actualizar las temperaturas totales
                if (temp[dia][i] < minTotal) {
                    minTotal = temp[dia][i];
                }
                if (temp[dia][i] > maxTotal) {
                    maxTotal = temp[dia][i];
                }
            }
            // Imprimir mínimas y máximas del día
            printf("\nDia %d: Minima = %.2f, Maxima = %.2f", dia + 1 , minDia, maxDia);
        }
 
        // Imprimir mínimas y máximas totales
        printf("\n\nTemperatura minima total = %.2f", minTotal);
        printf("\nTemperatura maxima total = %.2f", maxTotal);
}
```

### Actividad 3 P22

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>

int main(){
	
	int n;
	
	printf("Introduce el tomanyo del array: ");
	scanf("%d", &n);
	
	int array[n];
	
	printf("Introduce %d numeros enteros:\n");
	for(int i = 0; i <n ; i++){
		printf("Elemento %d: ", i + 1);
		scanf("%d", &array[i]);
	}
	printf("\n");
	
	printf("Array en orden inverso:\n");
    for (int i = n - 1; i >= 0; i--) {
        printf("%d ", array[i]);
	}
    printf("\n");
		
}
```

### Actividad 4 P22

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

### Actividad 5 P22

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

```c
#include <stdio.h>
#define MAX 100

int main(){
	int dim, fila, columna, k;
	int m1[MAX][MAX], m2[MAX][MAX], r[MAX][MAX];
	
	do{
		printf("Introduce la dimension: ");
		scanf("%d", &dim);
	}while(dim <= 0 || dim >= 100);
	
	//Matriz 1
	for( fila = 0; fila <dim ; fila++){
		for(columna = 0; columna <dim; columna++){
			printf("Introduce m1[%d][%d]: ", fila, columna);
			scanf("%d", &m1[fila][columna]);
		}
	}
	printf("\n");
	
	//Matriz 2
	for( fila = 0; fila <dim ; fila++){
		for(columna = 0; columna <dim; columna++){
			printf("Introduce m2[%d][%d]: ", fila, columna);
			scanf("%d", &m2[fila][columna]);
		}
	}
	
	for( fila = 0; fila <dim ; fila++){
		for(columna = 0; columna <dim; columna++){
			r[fila][columna] = 0;
		}
	}
	//Producto de matrices
	for( fila = 0; fila <dim ; fila++){
		for(columna = 0; columna <dim; columna++){
			r[fila][columna] = 0;
			for(k = 0 ; k < dim ; k++){
				r[fila][columna] = r[fila][columna] + (m1[fila][k] * m2[k][columna]);
			}
		}
		
	}
	//Mostrar en la pantalla
	for( fila = 0; fila <dim ; fila++){
		for(columna = 0; columna <dim; columna++){
			printf("%d ", m1[fila][columna]);
		}
		printf("\t");
		for(columna = 0; columna <dim; columna++){
			printf("%d ", m2[fila][columna]);
		}
		printf("\t");
		for(columna = 0; columna <dim; columna++){
			printf("%d ", r[fila][columna]);
		}
		printf("\n");
	}
	
}
```

### Actividad 5 P23

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

