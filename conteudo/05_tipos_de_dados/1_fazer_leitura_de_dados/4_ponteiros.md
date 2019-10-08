**ponteiro**

A utilização de ponteiros em linguagem C é uma das características que tornam a linguagem tão flexível e poderosa.

Ponteiros ou apontadores, são variáveis que armazenam o endereço de memória de outras variáveis.

Dizemos que um ponteiro “aponta” para uma varíável quando contém o endereço da mesma.

Os ponteiros podem apontar para qualquer tipo de variável. Portanto temos ponteiros para int, float, double, etc.

**Por que usar ponteiros?**
Ponteiros são muito úteis quando uma variável tem que ser acessada em diferentes partes de um programa.

Neste caso, o código pode ter vários ponteiros espalhados por diversas partes do programa, “apontando” para a variável que contém o dado desejado.

Caso este dado seja alterado, não há problema algum, pois todas as partes do programa tem um ponteiro que aponta para o endereço onde reside o dado atualizado.

Existem várias situações onde ponteiros são úteis, por exemplo:

* Alocação dinâmica de memória
* Manipulação de arrays.
* Para retornar mais de um valor em uma função.
* Referência para listas, pilhas, árvores e grafos.

**Sintaxe de declaração de ponteiro**
```c
tipo *nome_ponteiro;
```
Onde temos:

**tipo** : é o tipo de dado da variável cujo endereço o ponteiro armazena.

 ***nome_ponteiro** : O nome da variável ponteiro.

O asterisco * neste tipo de declaração determina que a variável será um ponteiro.

Exemplo de declaração de ponteiro:
```c
int *ptr;
```
**Exemplo: Programa utilizando ponteiro**
```c
#include <stdio.h>

int main(void){
	//valor é a variável que
	//será apontada pelo ponteiro
	int valor = 27;
	
	//declaração de variável ponteiro
	int *ptr;
	
	//atribuindo o endereço da variável valor ao ponteiro
	ptr = &valor;
	
	printf ("Utilizando ponteiros\n\n");
	printf ("Conteudo da variavel valor: %d\n", valor);
	printf ("Endereço da variavel valor: %d \n", &valor);
	printf ("Conteudo da variavel ponteiro ptr: %d \n", ptr);

	return(0);
}
```
**Tela de Execução**
```
Utilizando ponteiros

Conteudo da variavel valor: 27
Endereço da variavel valor: -1383940996 
Conteudo da variavel ponteiro ptr: -1383940996
```
Tela de execução do programa usando ponteiro

Explicação detalhada do código sobre ponteiros
```c
//valor é a variável que será apontada pelo ponteiro
int valor = 27;

//declaração de variável ponteiro
int *ptr;
```
Note que foi usado o operador * para designar que a variável ptr é um ponteiro. Como a intenção é armazenar o endereço da variável denominada valor que é uma variável do tipo int, o ponteiro também tem que ser do tipo int. Isto significa que vai apontar para uma variável do tipo inteiro.
```c
//atribuindo o endereço de valor ao ponteiro
ptr = &valor;
```
Para atribuir o endereço da variável valor ao ponteiro **ptr** utilizamos o operador de endereço **&**, pois estamos nos referindo ao endereço da variável valor e não ao conteúdo da mesma.
```c
   printf("Utilizando ponteiros\n\n");
   printf ("Conteudo da variavel valor: %d\n", valor);
   printf ("Endereço da variavel valor: %x \n", &valor);
   printf ("Conteudo da variavel ponteiro ptr: %x", ptr);
```
Foi utilizado **%x** para exibir o endereço e o conteúdo do ponteiro ptr, pois trata-se de um valor hexadecimal por ser endereço de memória.

[linguagemc](http://linguagemc.com.br/ponteiros-em-c/)