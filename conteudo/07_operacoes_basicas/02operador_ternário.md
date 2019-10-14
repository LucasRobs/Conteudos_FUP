**O operador ternário em C**
O operador ternário é uma alternativa para substituir o if…else em algumas situações por ser um comando bem enxuto.

Sintaxe:
```c
Condição ? verdadeiro : falso
```
Onde

Condição é a condição que será testada.

Verdadeiro é o que fazer quando a condição for verdadeira.

Falso é o que fazer quando a condição for falsa.

exemplo:
```c
#include <stdio.h>
int main (){
  int numero;
  
  printf("Digite um numero: ");
  scanf("%d",&numero);
  
  numero >= 0 ? numero++ : numero--;
  
  printf("O novo valor de numero e: %d",numero);
  
  return(0);
}
```

Explicação do código

numero >= 0 ? numero++ : numero–;

Neste código se o número for maior ou igual a zero será incrementado, caso contrário será decrementado de uma unidade.

Seria o equivalente a usar if:
```c
if (numero  > = 0)
   Numero ++;
else
   Numero --;
```