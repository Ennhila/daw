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

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

