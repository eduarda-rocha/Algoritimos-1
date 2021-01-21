
* Menu básico de Lanchonete

```
/* Escrever um algoritmo que leia o código do item pedido, a quantidade e calcule o valor a ser pago
 por aquele lanche. Considere que a cada execução somente será calculado um item.*/
 
#include<stdio.h>
#include<locale.h>
#include<stdlib.h>

int main(){
	setlocale(LC_ALL,"Portuguese");
	
	int codigo, quantidade;
	
	do{
	
	printf ("\n\nMenu: \n100-Cachorro-quente \n101-Bauru com ovo \n102-Bauru simples \n103-Hamburguer \n104-Cheeseburguer \n105-Refrigerante \n0-Sair \nInsira o código: ");
	scanf ("%d", &codigo);
	printf ("\nInsira a quantidade de lanche: ");
	scanf ("%d", &quantidade);
	
	switch (codigo){
		
		case 100:
			printf ("O valor a ser pago por %d Cachorro-quente é: %0.2f", quantidade, quantidade*1.2);
			break;
		case 101:
			printf ("O valor a ser pago por %d Bauru com ovo é: %0.2f", quantidade, quantidade*1.3);
			break;
		case 102:
			printf ("O valor a ser pago por %d Bauru simples é: %0.2f", quantidade, quantidade*1.4);
			break;
		case 103:
			printf ("O valor a ser pago por %d Hamburguer é: %0.2f", quantidade, quantidade*1.5);
			break;
		case 104:
			printf ("O valor a ser pago por %d Cheeseburguer é: %0.2f", quantidade, quantidade*1.6);
			break;
		case 105:
			printf ("O valor a ser pago por %d Cachorro-quente é: %0.2f", quantidade, quantidade*1.7);
			break;
		case 0:
			printf ("Finalizado!");
			break;
		default:
			printf("ERRO. Digite novamente");
	}
 }while(codigo!=0);
return 0;
}
```