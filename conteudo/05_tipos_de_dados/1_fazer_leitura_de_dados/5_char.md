**char**

O tipo char é utilizado para representar caracteres. Um caractere é representado através de um byte na memória. Lembre-se que um byte tem 8 bits, ou seja, é possível representar 256 números (ou no caso, codificar até 256 caracteres distintos). A linguagem C utiliza esse número como um índice na tabela ASCII. 

Para ler e imprimir caracteres, utilize **'%c'** no scanf e no printf. Quando uma tecla é digitada (lida pelo scanf) o código correspondente à tecla é traduzido para o número binário correspondente, e armazenado na variável utilizada no scanf. Quando uma variável caractere é utilizada no printf, esse número é utilizado para imprimir o caractere correspondente na tabela ASCII.

**Exemplo :**

```c
#include <stdio.h>

int main () {
    char c1; // apenas criando
    char c2 = 'X'; //criando e iniciando
    scanf("%c", &c1); // lendo um char
    printf("%c", c1); // printando um char
}
```
[ime.usp](https://www.ime.usp.br/~elo/IntroducaoComputacao/Caracter.htm)