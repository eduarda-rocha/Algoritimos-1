* Media de aluno com mensagem aprovado ou reprovado

```
/*Calcule a média aritmética das 3 notas de um aluno e mostre, além do valor da média, uma mensagem de "Aprovado", caso a média seja igual 
ou superior a 6, ou a mensagem "reprovado", caso contrário */

#include<stdio.h>
#include<stdlib.h>

int main(){
	
	float provas[3], media;
	
	for(int i=0; i < 3; i++){
		printf("\nEntre com a nota da prova %d: ",i+1);
		scanf("%f", &provas[i]);
	}
	
	media = (provas[0] + provas[1] + provas[2])/3;
	
	if (media > 6){
		printf ("\nAluno aprovado com media: %0.2f", media);
	}
	else{
		printf ("\nAluno reprovado com media: %0.2f", media);
	}	
		
	return 0;
	
}
``` 