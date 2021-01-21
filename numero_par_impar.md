* Número par ou ímpar, positivo ou negativo.

```
/*Faça um algoritmo que leia um nº inteiro e mostre uma mensagem indicando se este número é par ou ímpar, e se é positivo ou negativo.*/

#include<stdio.h>
#include<locale.h>

int main (){
	setlocale(LC_ALL, "Portuguese");
	
	int numero;
	
	printf("Insira um número inteiro: ");
	scanf("%d",&numero);
	
	if(numero%2==0){
		printf("\nO número %d é par.", numero);
	}
	else{
		printf("\nO número %d é ímpar.", numero);
	}
	if (numero>=0){
		printf ("\nO número %d é positivo.", numero);
	}
	else{
		printf ("\nO número %d é negativo", numero);
	}
	return 0;
}
```