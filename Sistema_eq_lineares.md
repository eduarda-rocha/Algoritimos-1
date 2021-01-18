* Sistema de equações lineares 
```
/* Sistema de equaçoes lineares do tipo ax+by=c e dx+ey=f
Escreva um algoritmo que lê os coeficientes a,b,c,d,e e f e calcula e mostra os valores de x e y */
#include<stdio.h>
#include<locale.h>

int main (){
	setlocale(LC_ALL,"Portuguese");
	
	float a, b, c, d, e, f;
	float valor_x, valor_y;
	
	printf ("Entre com o primeiro coefiente (a): ");
	scanf ("%f",&a);
	printf ("Entre com o segundo coefiente (b): ");
	scanf ("%f",&b);
	printf ("Entre com o terceiro coefiente (c): ");
	scanf ("%f",&c);
	printf ("Entre com o quarto coefiente (d): ");
	scanf ("%f",&d);
	printf ("Entre com o quinto coefiente (e): ");
	scanf ("%f",&e);
	printf ("Entre com o sexto coefiente (f): ");
	scanf ("%f",&f);
	
	valor_x = (c*e - b*f)/(a*e - b*d);
	valor_y = (a*f - c*d)/(a*e - b*d);
	
	printf ("Os valores de X e Y são respectivamente: %0.1f e %0.1f", valor_x, valor_y);
	return 0;

}
```