* Média ponderada de três notas
```
// media ponderada tres notas

#include<stdio.h>
#include<locale.h>

int main(){
	
	setlocale(LC_ALL, "Portuguese");
	
	float notaP1, notaP2, notaP3, media;
	
	printf ("Entre com a nota da P1: ");
	scanf ("%f",&notaP1);
	printf ("Entre com a nota da P2: ");
	scanf ("%f",&notaP2);
	printf ("Entre com a nota da P3: ");
	scanf ("%f",&notaP3);
	
	media = (notaP1*2 + notaP2*3 + notaP3*5)/10;
	
	printf("A media do aluno é: %0.1f ", media);
	return 0;
	
}
```