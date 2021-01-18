
* Distância entre dois pontos 
```
#include<stdio.h>
#include<math.h>

int main (){
	
	int x1, x2, y1, y2;
	float distancia;
	
	
	printf("Insira as coordenadas de x1 e y1 do primeiro ponto: ");
	scanf("%d%d",&x1,&y1);
	printf ("Insira as coordenadas de x2 e y2 do segundo ponto: ");
	scanf("%d%d",&x2,&y2);
	
	distancia = sqrt((pow((x2-x1),2)) + (pow((y2-y1),2)));
	
	printf("A distancia entre o ponto A e B é: %f", distancia);
	
	return 0;
	
}
```
 
