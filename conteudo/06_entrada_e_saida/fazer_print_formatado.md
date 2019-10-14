entrada e saída de dados  em linguagem C utilizando as funções scanf () e printf().

**Saída de dados**

Chamamos de saída de dados a exibição de textos ou valores de variáveis no vídeo.

**A função printf()**
O comando usado para exibir valores na tela é a função **printf()**.

**Sintaxe Básica**
```c
printf(“Mensagem a ser escrita na tela”);
```
Também é possível mostrar texto e valores de variáveis usando argumentos.

**Sintaxe:**
```c
printf(“Mensagem a ser escrita na tela”, lista de argumentos);
```
Exemplo de mensagem que inclui o valor de uma variável:
```c
printf(“Total a pagar: R$ %f”, total);
```
onde:

%f representa o local onde será escrita uma variável float
total é a variável float que será mostrada na posição marcada por %f

**Entrada de dados**
Tem por função efetuar a leitura de dados de uma fonte externa.

A  função scanf()
É utilizada para fazer a leitura de dados formatados via teclado.

Sintaxe:

scanf(“expressão de controle”, lista de argumentos);

Exemplo:

scanf(“%f”, &salario);

Explicação: este comando efetua uma leitura do teclado onde é esperada uma variável float (indicada por “%f”). O valor lido será armazenado no endereço da variável salário.

Na lista de argumentos devemos indicar os endereços das variáveis. Para fazer isso adicionamos o símbolo  “&”  como prefixo na frente do nome da variável.

**controle de casas decimais**

No momende de printar um float com %f. coloque %.2f
(o número antes do f define o número de casas decimais)
```c
#include<stdio.h>
int main(){
float a = 1.77777;
printf("%.2d\n", a);
}
```
saída : 
1.77

**controle de zeros à esquerda**

Preenchendo com 3 zeros por exemplo temos que 1 fica 001, 50 fica 050 e 200 fica inalterado. Pra que fazer isso? Geralmente para exibir melhor matrizes.

```c
#include<stdio.h>
int main(){
int a = 15;
printf("%03d\n", a);
printf("%04d\n", a);
}
```
Isso dá uma saída:

015
0015

[linguagemc](http://linguagemc.com.br/operacoes-de-entrada-e-saida-de-dados-em-linguagem-c/)