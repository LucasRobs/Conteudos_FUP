**struct**

Uma struct é uma variável especial que contém diversas outras variáveis normalmente de tipos diferentes.

As variáveis internas contidas pela struct são denominadas membros da struct.

Podemos dizer que as structs da linguagem C são o equivalente ao que se denomina registros em outras linguagens de programação.

Sintaxe:
```c
struct <identificador>
{
 <listagem dos tipos e membros>;
}
struct <identificador> <variavel>;
```
Exemplo de declaração de uma struct
```c
struct ficha_de_aluno
{
char nome[50];
char disciplina[30];
float nota_prova1;
float nota_prova2;
};
struct ficha_de_aluno aluno;
```
Neste exemplo criamos a struct ficha_de_aluno.

Depois de criar a struct precisamos criar a variável que vai utiliza-la.

Para tanto criamos a variável aluno, que será do tipo ficha_de_aluno.
```c
struct ficha_de_aluno aluno;
```
Agora vejamos um programa que utiliza uma struct.
```c
#include <stdio.h>
int main(void){
	/*Criando a struct */
	struct ficha_de_aluno
	{
		char nome[50];
		char disciplina[30];
		float nota_prova1;
		float nota_prova2;
	};
	
	/*Criando a variável aluno que será do
	tipo struct ficha_de_aluno */
	struct ficha_de_aluno aluno;
	
	printf("\n---------- Cadastro de aluno -----------\n\n\n");
	
	printf("Nome do aluno ......: ");
	fflush(stdin);
	
	/*usaremos o comando fgets() para ler strings, no caso o nome
	do aluno e a disciplina
	fgets(variavel, tamanho da string, entrada)
	como estamos lendo do teclado a entrada é stdin (entrada padrão),
	porém em outro caso, a entrada tambem poderia ser um arquivo */
	
	fgets(aluno.nome, 40, stdin);
	
	printf("Disciplina ......: ");
	fflush(stdin);
	fgets(aluno.disciplina, 40, stdin);
	
	printf("Informe a 1a. nota ..: ");
	
	scanf("%f", &aluno.nota_prova1);
	
	printf("Informe a 2a. nota ..: ");
	scanf("%f", &aluno.nota_prova2);
	
	printf("\n\n --------- Lendo os dados da struct ---------\n\n");
	printf("Nome ...........: %s", aluno.nome);
	printf("Disciplina .....: %s", aluno.disciplina);
	printf("Nota da Prova 1 ...: %.2f\n" , aluno.nota_prova1);
	printf("Nota da Prova 2 ...: %.2f\n" , aluno.nota_prova2);
	
	return(0);
}
```
[linguagemc](http://linguagemc.com.br/struct-em-c/)