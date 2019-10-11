**string**
Usando scanf

A função scanf permite fazer leitura de strings usando %s.

Em relação ao uso de scanf para armazenar string devemos observar duas coisas:

A função scanf realiza a leitura até encontrar um espaço, depois encerra a leitura e coloca o caracter terminador \0.
A variável que vai armazenar a string não necessita ser precedida por &.
Exemplo de utilização do scanf:

scanf(“%s”,nome);

**Exemplo: Usando scanf para receber uma string.**
 ```c
 #include <stdio.h>
int main(){
  char nome[61];//declarando uma string
  
  printf("Digite seu nome: ");
  scanf("%s",nome); // para ler não precisa de '&' pois é um ponteiro
  
  printf("O nome armazenado foi: %s", nome);

  return 0;
}
 ```