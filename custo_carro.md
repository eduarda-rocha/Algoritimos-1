* Custo de um carro ao consumidor
```
/*Supondo que a percentagem do distribuidor seja de 28% e os impostos de 45%, escrever um algoritmo que leia o custo de fábrica
 de um carro e escreva o custo ao consumidor */
 
#include<stdio.h>
#include<locale.h>

int main(){
	setlocale (LC_ALL, "Portuguese");
	
	float custo_fabrica, custo_consumidor;
	
	printf ("Insira o valor do custo de fábrica do carro: ");
	scanf ("%f",&custo_fabrica);
	
	custo_consumidor = (custo_fabrica + 0.28*custo_fabrica + 0.45*custo_fabrica);
	
	printf ("O custo ao Consumidor é de: %0.2f", custo_consumidor);
	
	return 0;
}
```