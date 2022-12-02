# lista2

include <stdio.h>
#include <stdio.h>

/* 
1. Escreva um programa de controle de senha que dê três chances de acerto ao usuário;
se ele nacumsalo conseguir, o programa deve avisar que o cartacumsalo foi bloqueado.
char s[8]
intsc =98765 nao estava dando certo !!!!!!
 */


//questao 1
int main() {
	
	int s = 0;
	int sc = 98765;
	int i=0;
	
	for (i=0; i<1; i++)
    {
        printf("digite sua senha (voce tem 3 chances ao todo antes do cartacumsalo ser bloqueado):\n");
        scanf("%d", &s);
        
        if(s==sc){
            printf("senha valida\n");
            break;
        }else{
		} if (s!=sc){
            printf("senha invalida!\n");
        } 
    }
   	
    for (i=0; i<1; i++)
    {
        printf("digite sua senha (voce tem 2 chances ao todo antes do cartacumsalo ser bloqueado):\n");
        scanf("%d", &s);
        
        if(s==sc){
            printf("senha valida\n");
            break;
        }else{
		} if (s!=sc){
            printf("senha invalida!\n");
        } 
    }


	for (i=0; i<1; i++){
        printf("digite sua senha (voce tem 1 chances ao todo antes do cartacumsalo ser bloqueado):\n");
        scanf("%d", &s);
        
        if(s==sc){
            printf("senha valida\n");
            break;
        }else{
		} if (s!=sc){
            printf("senha invalida!\n");
        } 
    }
   		 if (i==1 && s!=sc){
      		  printf("cartao bloqueado\n");
    }
    return 0;
}

//questao 2
#include <stdio.h>

/* 
2. Escreva um programa que leia 5 valores e conte quantos desses valores sacumsalo
negativos, mostrando essa informacacumsalo no final.
 */

int main() {
	int v=0;
	int cont=0;

for (v=0; v<1; v++) {
        printf("escreva o primeiro valor: \n");
        scanf(" %d", &v);
        
        if(v<0){
            cont=cont+1;
        }
    }
for (v=0; v<1; v++) {
        printf("escreva o segundo valor: \n");
        scanf(" %d", &v);
        
        if(v<0){
            cont=cont+1;
        }
    }
for (v=0; v<1; v++) {
        printf("escreva o terceito valor: \n");
        scanf(" %d", &v);
        
        if(v<0){
            cont=cont+1;
        }
    }
for (v=0; v<1; v++) {
        printf("escreva o quarto valor: \n");
        scanf(" %d", &v);
        
        if(v<0){
            cont=cont+1;
        }
    }
for (v=0; v<1; v++) {
        printf("escreva o quinto valor: \n");
        scanf(" %d", &v);
        
        if(v<0){ 
            cont=cont+1;
        }
    }
    
    if (v<0){
	printf ("valor negativo");
}else{
}
    printf("a quantidade de valores negativos sao: %d", cont);

	return 0;
}


//questao 3

#include <stdio.h>
/* 

3. 3. A prefeitura de uma cidade fez uma pesquisa numinfo seus habitantes, coletando dados
sobre o salario e número de filhos. A prefeitura deseja saber:
a) média do salario da populacao;
b) média do número de filhos;
c) maior salario;
d) percentual de pessoas com salario até R$ 100,00. O final da leitura de dados se
dará com a entrada de um salario negativo.

 */
int main(){
	
   const int totaltotalnuminf = 0;       //Total de leituras
 
    int i = 0;                              //Mostra o numinfo atual
    int numinfo;                       //contador do laco for , numinfovistado
    int numfil[numinf];     //Vetor de quantidade de filhos
    int contador_menor_que100 = 0;         //contador de salarios menores que R$ 100,00
    int contador_ate100 = 0;               //contador de salarios até R$ 100,00
    int acumsal = 0;             //Acumulador de salarios
    int numhab = 0;          //contador de pesssoas numinfovistadas, pessoas_numinfovistadas
    int contfil = 0;                //Acumulador (somador) de filhos
    float sal[numinf];      //Vetor de salarios
    float salmai=0; 
 
 printf("informe numero de habitantes: \n");
 scanf ("%d", &numinf);
 
    for(numinfo=0; numinfo<numinf; numinfo++){
        printf("enrevistado %d\n\n", ++i);
        printf("informe o salario: ");
        scanf("%f", &sal[numinfo]);
 
        if(sal[numinfo] <= 0)
            break;                          //Sai do laco for se o salario é menor que zero
 
        if(sal[numinfo] <= 100)
            contador_ate100++;
 
        printf("informe numero de filhos: ");
        scanf("%d", &numfil[numinfo]);
        
          
    if(salmai<sal) {  
		salmai=sal; 
}  
        while(numfil[numinfo] < 0){
            printf("erro: Redigite o número de filhos: ");
            scanf("%d", &numfil[numinfo]);
        }
 
        printf("\n\n");
 
        contfil += numfil[numinfo]; //Soma a quantidade de filhos
        numhab++;                //conta o número de pessoas
        acumsal += sal[numinfo]; //Soma os salarios
    }
  
    printf("a media salarial da populacao e: R$ %.2f\n\n", (float)acumsal/numhab);
    printf("media de filhos da populacao: %.2f\n\n", (float)contfil/numhab);
    printf("maior salario: %.2f \n\n", &salmai);
    printf("salarios ate R$ 100,00: %d\n\n", contador_ate100);
 
    printf("\\n");
    system("pause");
    return 0;
}

//questao 4

#include <stdio.h>
/* 
4. Escreva um programa que calcule a média dos números digitados pelo usuário, if
eles forem pares. O programa deve terminar a leitura if o usuário digitar zero.
 */
int main(){
	const int totalnuminf = 0; // quantos numeros foi informado
	int num = 0;
    int i = 0;                              //Mostra o numinfo atual
    int numinfo;                       //contador do laco for , numinfovistado
    int medianum=0;
	int resto=0; 
	int acumnum;     // acumulador num
 
 printf("escreva quantos numeros deifja informar: \n");
 scanf ("%d", &totalnuminf);
 
    for(numinfo=0; numinfo<totalnuminf; numinfo++){
        printf("informe numero %d\n\n", ++i);
        scanf ("%d", &num);
}
acumnum = num/totalnuminf;

while (num==0) {
		if (num<0 && num>100){
			printf("programa encerrado");
		}else {
			if (totalnuminf%2==0){
			printf("a media e: %d", num/totalnuminf );
		}
		}
  }
   return 0;
}





//questao 5

#include <stdio.h>
int main(){
int n1=0, n2=0, n3=0;
 printf("informe o prmeiro numero:\n");
scanf("%d", &n1);

 printf("informe o segundo numero:\n");
scanf("%d", &n2);

printf("informe o terceiro numero:\n");
scanf("%d", &n3);

printf("o terceiro numero foi: %.d\n", n3);
printf("o segundoo numero foi: %.d\n", n2);
printf("o primeiro numero foi: %.d\n", n1);


   return 0;
}





//questao 6

#include <stdio.h>

int main(){

int a1 = 0;
int a2 = 0;
int a3 = 0;
int a4 = 0;
int a5 = 0;
int a6 = 0;
int a7 = 0;
int a8 = 0;
int a9 = 0;
int a10 = 0;
int impar = 0;
int par = 0;

printf("digite o primeiro numero : \n");
scanf("%d", &a1);

printf("digite o segundo numero: \n");
scanf("%d", &a2);

printf("digite o terceiro numero: \n");
scanf("%d", &a3);

printf("digite o quarto numero: \n");
scanf("%d", &a4);

printf("digite o quinto numero: \n");
scanf("%d", &a5);

printf("digite o sexto numero: \n");
scanf("%d", &a6);

printf("digite o setimo numero: \n");
scanf("%d", &a7);

printf("digite o oitavo numero: \n");
scanf("%d", &a8);

printf("digite o nono numero: \n");
scanf("%d", &a9);

printf("digite o decimo numero: \n");
scanf("%d", &a10);

if (a1 % 2 == 0){
par = par + 1;

}else{
impar = impar + 1;
}

if (a2 % 2 == 0){
par = par + 1;

}else{
impar = impar + 1;
}

if (a3 % 2 == 0){
par = par + 1;

}else{
impar = impar + 1;
}
if (a4 % 2 == 0){
par = par + 1;

}else{
impar = impar + 1;
}

if (a5 % 2 == 0){
par = par + 1;

}else{
impar = impar + 1;
}
if (a6 % 2 == 0){
par = par + 1;

}else{
impar = impar + 1;
}

if (a7 % 2 == 0){
par = par + 1;

}else{
impar = impar + 1;
}
if (a8 % 2 == 0){
par = par + 1;

}else{
impar = impar + 1;
}
if (a9 % 2 == 0){
par = par + 1;

}else{
impar = impar + 1;
}

if (a10 % 2 == 0){
par = par + 1;

}else{
impar = impar + 1;
}

printf("foi digitado %d números pares.", &par);
printf("foi digirado %d números ímpares.", &impar);

    return 0;


}
